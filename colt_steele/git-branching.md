# Git Branching

- If we make changes on 1 branch, they do not impact the other branches (they exist in isolation).

## Git HEAD

- HEAD is simply a pointer that refers to the current location in the repository.
- HEAD points to a particular **branch reference**.
- HEAD always points to the latest commit made on the master branch.
- If switch branch, HEAD will switch to the new branch.

## Git Branch

- `git branch`:
  - view the existing branches.
  - The default branch in every git repo is master, can configure this.
- `git branch <branch-name>`
  - make a new branch **based upon the current HEAD**
  - just creates the branch. does not switch to that branch (HEAD stays the same).
    - `(HEAD -> master, bugfix)`

## Git Switch

- `git switch <branch name>`
  - to switch to a new branch.
- `git switch -c <branch name>`
  - the `-c` flag to create a new branch and switch to it all in one go
  - `-c`: create

## Git Checkout

- `git checkout <branch name>`
  - switch branches (old school way of switching)
  - checkout has more functionalities than git switch.
- `git checkout -b <branch name>`
  - create a new branch and switch to it all in one go.

## Switching Branches with Unstaged Changes

- If you modified an old file, need to add & commit or stash those changes before switching branches.
- If you created a new file, it is possible to switch branches.
  - However, it is recommended to add & commit or stash the changes before switching branches.

## Deleting & Renaming Branches

- `git branch -D <branch name>`
  - delete a branch even if it has not been fully merged.
  - must not be on the branch to delete it.
  - useful to delete a branch that contains work that you no longer need or want to keep. 
  - Similar to `git branch -d <branch name>` but it adds the `--force` tag.

- `git branch -m <branch name>`
  - rename a branch.
  - must be on the branch itself to rename it.

## HEAD & Refs

- HEAD refers to the current commit in the local repository.
- The HEAD pointer points to the current commit and determines which commit is considered the current commit.
- Can use the HEAD pointer to reference other commits in the repository, such as by using the syntax "HEAD~1" to refer to the commit that comes immediately before the current commit. 
- The HEAD pointer is like a cursor that points to the current position in the commit history of the repository and allows you to navigate and manipulate the commit history.



