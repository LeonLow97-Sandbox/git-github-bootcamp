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

- Add multiple stashes onto the stack of stashes. They will all be stahed in the order you added them.

```
git stash
    do some other stuff...
git stash
    do some other stuff...
git stash
```

- `git stash list`: to view all stashes

```git
stash@{0}: WIP on rainbow: dd6ad48 remove background color
stash@{1}: WIP on rainbow: dd6ad48 remove background color
stash@{2}: WIP on rainbow: dd6ad48 remove background color
stash@{3}: WIP on goodbye: d6f9c8d create index.html and app.css
```

# Applying and Clearing The Stash

- `git stash apply stash@{2}`: specify a particular stash
- `git stash drop stash@{2}`: remove a particular stash
- `git stash clear`: removes all stash
