# Summary of Git Commands

## Git Commit

| Git Command | Description |
|---------|-------------|
| Git repository | A workspace that tracks and manages the files within a folder. Can create as many repositories on your machine as needed, each with its own separate history and content. |
| `git status` | Gives information on the current status of a Git repository and its contents. |
| `git init` | Creates an empty Git repository or reinitializes an existing one. |
| Basic Git workflow | Involves making changes to files, adding those changes to the staging area using `git add`, and committing those changes using `git commit`. |
| `git commit` | Takes a snapshot of the Git repository at a specific point in time and requires a commit message to describe the changes being committed. |
| `git log` | Shows a list of all the commits made to a repository. |
| Atomic commits | Keep each commit focused on a single thing. |
| `git commit --amend` | Redo the previous commit and make changes to it. |
| `.gitignore` | Allows you to tell Git which files and directories to ignore in a given repository. |

## Git Branching

| Git Command | Description |
| --- | --- |
| `git branch` | View the existing branches. The default branch in every Git repository is "master," but this can be configured. |
|`git branch -v`|Shows the branches and the last commit of each branch.|
| `git branch <branch-name>` | Create a new branch based on the current HEAD. This command does not switch to the new branch; the HEAD remains unchanged. |
| `git switch <branch-name>` | Switch to an existing branch. |
| `git switch -c <branch-name>` | Create a new branch and switch to it all in one go. The `-c` flag stands for "create." |
| `git checkout <branch-name>` | Switch to an existing branch (old school way of switching branches). The `git checkout` command has more functionality than `git switch`. |
| `git checkout -b <branch-name>` | Create a new branch and switch to it all in one go. |
| `git branch -D <branch-name>` | Delete a branch, even if it has not been fully merged. You must not be on the branch to delete it. This command is useful for deleting a branch that contains work that you no longer need or want to keep. This command

