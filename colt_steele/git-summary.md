# Summary of Git Commands

## Git Commit

| Concept | Description |
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

| Concept | Description |
|---------|-------------|
| Git HEAD | A pointer that refers to the current location in the repository. Points to the latest commit made on the current branch. Can be switched to a new branch by changing HEAD's reference. |
| Git branch | A separate line of development in a Git repository. The default branch is `master`, but new branches can be created using the `git branch` command. |
| Git switch | A command to switch to a new branch. Can be used with the `-c` flag to create a new branch and switch to it all in one go. |
| Git checkout | A command to switch to a new branch. Can be used with the `-b` flag to create a new branch and switch to it all in one go. |
| Switching branches with unstaged changes | If you have modified an old file and want to switch branches, it is a good idea to either commit those changes or stash them before switching branches. If you have created a new file, it is recommended to either commit or stash the changes before switching branches. |
| Deleting & renaming branches | Can use the `git branch -d <branch-name>` command to delete a branch, and the `git branch -m <old-branch-name> <new-branch-name>` command to rename a branch. |
| HEAD & refs | HEAD is a special reference that always points to the current branch, while other references are used to point to specific commits. |
