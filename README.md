# Git Tutorial
![home](./assets/git-flow.PNG)

A repo about git tutorial. It contains essential git commands with both local machine and remote server

## Local machine
- `git init .` -> initialize a local working directory
- `git add .` -> add to staging area
- `git commit -m "message"` -> commit to history (includes a bunch of commit)

## Remote server
An online platform to host and collaborate on git repos

- `git push` -> push changes to the `main` branch in remote server
- `git pull` -> pull new changes from remote server

## Show changes and status
- `git diff` -> show the current difference
- `git status` -> check working directory status
- `git log --oneline` -> see history(past commits)
- `git show history-id` -> show the changes from that commit

# Git Branches FLow
![home](./assets/flow-of-branches.png)
A branch represent an independent line of development

- `git branch -a` -> show a list of branches in the repo
- `git checkout -b branch-name` -> create new branch and move to that branch
- `git branch -d branch-name` -> delete that branch
- `git checkout branch-name` -> change to the that branch
- `git checkout -` -> change back to the previous branch

# Git Rebase
Action normally takes place when there are changes from main/master on remote server while the local machine is not up to date.

## Steps1
1. Put local changes aside
2. Merge current base and new changes from remote server together
3. Add local changes on the top.

- `git pull -r origin main` -> pull and rebase
- `git push -f` -> force push
