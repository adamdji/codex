# Git Cheat Sheet

## Misc

### Move back from `HEAD` to specific commit

- `HEAD~ (Parent of HEAD)`
- `HEAD~~ (Parent of parent of HEAD)`

## Branching CommandsW

### Branch

#### View Merged and unmerged branches

1. `git branch --merged`
2. `git branch --no-merged`
3. `git branch -r --no merged`

### Rebase

#### Rebase pull with autostash

`git pull --rebase --autostash`

## Commit Commands

### Cherry-Pick

#### Apply latest commit from one branch to another

`git cherry-pick -`

#### Copy the changes of the referenced commit to the `HEAD` of the current branch (as a new commit). Good way to revert a revert

`git cherry-pick head~~~`

## Difference Commands

### Diff

#### View file changes of diff

`git diff --stat (--staged)`

### Outputs the changes between `head~` and `HEAD` of the current branch. If only one commit is provided, other commit is assumed to be `HEAD`

`git diff head~`

#### Outputs the changes between the first commit and the second commit

`git diff head~~~..head~~`

### Git Show

#### Show changes in first parent

`git show head~`

#### Show changes in latest commit of specific branch

`git show branch-name`

#### Outputs the list of files changed in the commit with the given hash

`git show 19e771 --stat`

#### Outputs the changes made to the `README.md` file in the `HEAD` commit of the `my-feature` branch

`git show my-feature -- README.md`

#### Outputs the changes made to the `README.md` file in the `19e771` commit

`git show 19e771 -- README.md`

#### Outputs the contents of the `README.md` file as defined in the `19e771`commit

`git show 19e771:README.md`

## Git Remote Commands

### Remote

#### Prune remote-tracking branches

`git fetch --prune`
`git remote prune origin --dry-run`
`git remote prune origin`

### Push

### Delete remote branch

`git push origin local:remote`
`git push --delete origin branch-name`
`git push -d origin branch-name`
