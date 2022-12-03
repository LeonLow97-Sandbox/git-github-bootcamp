# Basics of Git: Adding & Committing

- [Slides](https://www.canva.com/design/DAEPH_Lq4Wk/Wp_d5Rvk_OjVvgPH0xmzhg/view?utm_content=DAEPH_Lq4Wk&utm_campaign=designshare&utm_medium=link&utm_source=sharebutton)

# What is a Git Repo?

- Git repo is a workspace which tracks and manages files within a folder.
- Anytime we want to use Git with a project, app, etc. need to create a new git repository.
- Can have as many repos on our machine as needed, all with separated history and content on our machine.

## `git status` and `git init`

- `git status`: gives information on the current status of a git repository and its contents.
- `git init`: create an empty Git repository or reinitialize an existing one.
  - creates a hidden file `.git`
  - hidden files begin with a `.`

---

# Git Basic Workflow

1. Work on Stuff
   - Make new files, edit files, delete files, etc.
2. Add Changes
   - Group specific changes together, in preparation of committing.
3. Commit
   - Commit everything that was previously added.

<img src="./pics/git-workflow.png" alt="Git Basic Workflow">

## `git add`

- `git add`: add specific files to the staging area.
- Syntax: `git add file1 file2`
- `git add .` stages all changes at once.

## `git commit`

- `git commit`: taking a snapshot of a git repository in time.
- Syntax: `git commit -m <commit_message>`
- Running `git commit` opens up VIM (try to avoid this).
- commit changes from the staging area. need to provide a commit message.
- When saving a file, we are saving the state of a single file.
- With Git, we can save the state of multiple files and folders together.

## `git log`

- `git log`: shows a list of all the commits made to a repository.
