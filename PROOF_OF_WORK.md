# Proof of Work

## git log --oneline

cb53442 (HEAD -> main, origin/main) Merge pull request #1 from anaszpro/development
b2bb8ef (origin/development, development) Resolve merge conflict between development and staging
8e53db8 (origin/staging, staging) Update deploy script for staging
23d00f6 Add tests step to deploy script
8ae69cb Initial commit with readme and deploy script


## 2. Reflection Questions


### Q1: Difference between Git (local tracking) and GitHub (cloud platform).

Git is a command-line tool installed on your computer that tracks changes in your files over time and manages local branches. GitHub is a cloud-based service that hosts Git repositories online so developers can share code. Git works entirely offline on your machine, while GitHub provides online collaboration features like pull requests, issue trackers, and code reviews.


### Q2: Explain 3 architecture stages: Working Directory, Staging Area, Local Repository.

The Working Directory contains the actual files on your machine that you are currently editing. The Staging Area (Index) acts as a checkpoint where you gather and review specific modified files using `git add` before committing them. The Local Repository is the hidden `.git` folder that stores the permanent history of all snapshots you save using `git commit`.


### Q3: Difference between git stash pop and git stash apply.

Both commands take temporary uncommitted work that was hidden away and bring it back to your active workspace. The command `git stash pop` restores the changes and immediately deletes that entry from the stash list. In contrast, `git stash apply` restores the changes while leaving a copy inside the stash list so you can reapply it elsewhere if needed.


### Q4: Difference between git fetch and git pull.

The command `git fetch` checks the remote repository and downloads any new changes, branches, or commits to your local system without modifying your active files. The command `git pull` does two things at once: it runs `git fetch` to grab the changes, and then immediately runs `git merge` to integrate them directly into your current working branch.

