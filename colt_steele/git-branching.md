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
- `git switch <branch name>`
    - to switch to a new branch.


## Git Switch

## Git Checkout

## Deleting & Renaming Branches

## HEAD & Refs
