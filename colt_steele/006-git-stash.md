# Git Stash Basics

- Changes in another branch are brought to the destination branch upon switching (no conflicts).
- Git doesn't allow switch if it detects potential conflicts.

# Git Stash

- Stashing uncommitted changes so that we can return to them later, without having to make unnecessary commits.
- `git stash`: helps save changes that are not ready to commit. Can stash changes and then come back to them later.
    - Running `git stash` will take all uncommitted changes (staged and unstaged) and stash them, reverting the changes in your working copy.
    - can also use `git stash save` instead.

# Git Stash Save

- `git stash save` similar to `git stash`

# Git Stash Pop

- `git stash pop`: remove the most recently stashed changes in the stash and re-apply them to the working copy.
    - pop in same branch or different branch.

# Git Stash Apply

- `git stash apply`: apply whatever is stashed away, without removing it from the stash. 
    - `git stash pop` is different because it removes it from the stash but `git stash apply` does not.
    - `git stash apply` useful if you want to apply stashed changes to multiple branches.

# Working with multiple stashes

# Applying and Clearing The Stash
