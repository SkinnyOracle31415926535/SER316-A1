#branch structure
- main : root branch of the working game
- dev : adds encouraging message for players
- feature1 : includes quit game with a negative number, play again loop, improved messages, and version comment
- feature2 : adds max attempts and a game over condition
- feature3 : hint system after 3 tries
- hotfix : fixes random number generator to include the max value in the range

## Learning Summary

### Merging vs. Rebasing

Merging joins two branches together by making a "merge commit". This shows both the past and proposed changes. Rebasing moves your commits so that they sit on top of the other branch. This makes the history look linear. Merging was done when merging dev and rebasing was done when feature2 and feature3 were done.

### Cherry-Picking

Cherry-picking is when you copy a specific commit from any branch and drop it into your current branch as a new commit. It creates a new copy with a new hash.

### Squashing Commits

Squashing commits combines multiple commits into one. This keeps the history readable.

### Resolving Merge Conflicts

A conflict happens when two branches both changed the same lines in the same file. It uses `<<<<<<<`, `=======`, `>>>>>>>` to let the user decide. You manually combine the changes and then `git add` the file and continue the merge.

### Branch Strategy

The branch strategy is the order you integrate branches.
