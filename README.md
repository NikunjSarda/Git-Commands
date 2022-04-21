# Git-Commands

## Cloning
* Simply clone
```bash
git clone <repo name>
```
* Clone a branch
```bash
git clone -b <branch-name> <repo name>
```

## Remotes
* Add a remote
```bash
git remote add <remote name> <remote url>
```
* Rmeove a remote
```bash
git remote remove <remote name>
```
* Show remote
```bash
git remote -v
```

## Stage Changes
* Stage changes
```bash
git add <changes>
```
* Stage hunks (May need to edit hunks with editor)
```bash
git add <changes> -p
```

## Commit Changes
* Commit (Opens editor for message)
```bash
git commit
```
* Fixup commit
```bash
git commit --fixup <commit id to fixup> -m <additional fixup message>
```

## Push changes
* Push to HEAD
```bash
git push <remote> HEAD
```
* Push to another branch
```bash
git push <remote> <commit>
```

## Pull changes
* Fetch+Merge from origin
```bash
git pull <remote> <HEAD>
```
* Just fetch from remote (Not merge)
```bash
git fetch
```
## Stashing
* Stash away unstaged
```bash
git stash
```
* Apply stash
```bash
git statsh pop
git statsh apply
```
* Show stash
```bash
git stash show
```
* Drop stash
```bash
git stash drop
```

## Diffs
* Basic diff
```bash
git diff <commit 1> <commit 2>
```
* Current unstaged changes
```bash
git diff
```
* Current unstaged on particular file
```bash
git diff -- <file>
```
* Staged changes
```bash
git diff --staged
```
* Staged changes on a particular file
```bash
git diff --staged -- <file>
```

## Rename
* Rename file in git tree
```bash
git mv <src> <dst>
```

## Checkout
* Checkout a branch (pre-existing)
```bash
git checkout <branch>
```
* Create and checkout to a new branch
```bash
git checkout -b <branch>
```
* Reset unstaged changes
```bash
git checkout .
```
* Reset unstaged changes on a file
```bash
git checkout -- <file>
```
* Reset Local Commits, commits not pushed
```bash
git reset --hard origin/<branch_name>
```
## Configs
* Rebase
```bash
git config pull.rebase true
```
