# Git Merge

- Incorporate changes from one branch to another.
- use the `git merge` command.
- Merge branches, not specific commits.
- Always merge to the current HEAD branch.

## Fast Forward Merges

- The HEAD pointer is simply **moved forward to point to the latest commit** in the source branch.
- Fast Forward Merges are often used to merge changes from a feature branch back into the main branch (single source of truth).
- E.g., To merge the bugfix branch into the master branch
  1. Switch to the branch you want to merge the changes into (the receiving branch)
     - `git switch master`
  2. Use the `git merge` command to merge changes from a specific branch into the current branch.
     - `git merge bugfix` 

## Git Merge & Merge Commits

- 

## Resolving Merge Conflicts

## Using VSCode To Resolve Conflicts
