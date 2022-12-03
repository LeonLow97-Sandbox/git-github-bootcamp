# What is Git?

- Version Control System

## Version Control

- Version control is software that **tracks and manages changes** to files over time.
- Version control system generally allow users to revisit earlier version of the files, compare changes between versions, undo changes, ...

## What does Git do?

- Track changes across multiple files
- Compare versions of a project
- "Time travel" back to old versions
- Revert to a previous version
- Collaborate and share changes
- Combine changes

## GitHub

- Github is a service that hosts Git repositories in the cloud and makes it easier to collaborate with other people
- Do need to sign up for an account to use GitHub.
- An online place to share work that is done using Git.

## Git is (Primarily) a Terminal Tool

- Git was created as command-line tool.
- To use it, we run various git commands in a Unix shell.

# Git GUI

- GitHub Desktop
- SourceTree
- Tower
- GitKraken
- Ungit

# Configuring Git

- Name
- Email

```
// Check if you have a name or email
git config user.name
git config user.email

// Set name or email
git config --global user.name "Leon"
git config --global user.email "leon@email.com"
```

# Terminal - Navigation

|Terminal Commands|Description|
|:-:|:-:|
|`ls`, `ls <folder_name>`|shows all the files in the current directory.|
|`ls -a`|list all files (including hidden files)|
|`open .`, `open <folder_name>`|open the current folder in path finder (works for _mac_).|
|`start .`|open the current folder in path finder (works for _windows_).|
|`pwd`|"print working directory", prints the path to the working directory (where you currently are)|
|`cd`|"change directory", to change and move between folders.|
|`cd ..`|to move back one directory.|
|`code .`|open vscode from the current working directory.|

# Terminal - Creating Files and Folders

|Terminal Commands|Description|
|:-:|:-:|
|`touch <file_name>`|create a _file_ (or multiple), e.g., `touch red.txt orange.py yellow.pdf`|
|`mkdir <folder_name>`|create a new directory (or directories)|

# Terminal - Deleting Files and Folders

|Terminal Commands|Description|
|:-:|:-:|
|`rm <file_name>`|delete a file or files **permanently**.|
|`rm -rf <directory>`|delete a directory (`r` = recursive, `f` = force)|





























