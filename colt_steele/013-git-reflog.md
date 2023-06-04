# Git Reflogs - Retrieving "Lost" Work

- Git keeps a record of when the tips of branches and other references were updated in the repo.
- Can view and update these reference logs using the git reflog command.

<img src="./pics/HEAD-reflog.png" alt="HEAD" width="50%" />

## Limitations of Git Reflog

- Git only keeps reflogs **locally**, not shared with collaborators.
- Reflogs also expire. Git cleans out old entries after around 90 days (configurable).

## `git reflog`

- `git reflog` or `git reflog show` or `git reflog show HEAD`
    - shows the log of a specific reference (default to HEAD).
- `git reflog show <branch_name>`
    - view the logs for the tip of the specified branch