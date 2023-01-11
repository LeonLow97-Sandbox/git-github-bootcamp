# Git Diff 

- `git diff`: lists all the changes in our working directory that are NOT staged for the next commit. Compares staging area and working directory.
- Often use `git diff` along commands like `git status` and `git log`.
- `git diff HEAD`: lists all changes in the working tree since the last commit. (compares working directory with staging/unstaging area).
- `git diff --staged` or `git diff --cached`: list the changes between the staging area and the last commit.

# Diffing Specific Files

- View the changes within a specific file by providing git diff with a filename.
- `git diff HEAD [filename]`
- `git diff --staged [filename]`

# Diffing Branches

# Diffing Commits


# Git diff --staged