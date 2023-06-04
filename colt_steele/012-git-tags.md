# Git Tags: Marking Important Moments in History

## Git Tags

- Tags are pointers that refer to particular points in Git history.
- Often used to mark version releases in projects (v4.1.0, v4.1.1, etc.)
- Tags are like branch references that do not change.
    - Once a tag is created, it always refers to the same commit.
    - Just a label for a commit.

## 2 Types of Git Tags

1. Lightweight tags
    - Just a name/label that points to a particular commit.
2. Annotated tags
    - store extra meta data including the author's name and email, the date and a tagging message (like a commit message).

## Semantic Versioning

- Semantic versioning spec outlines a standardized versioning system for software releases.
- It provides a consistent way for developers to give meaning to software releases.
    - "how big of a change is this release?"
- Version consist of 3 numbers separated by periods. E.g., `2.4.1`
    - First number: Major Release
    - Second number: Minor Release
    - Third number: Patch Release
- **Patch releases** normally do not contain new features or significant changes. They typically signify bug fixes and other changes that do not impact how the code is used.
- **Minor release** signify that new features or functionality have been added, but the project is still backwards compatible. No breaking changes. The new functionality is optional and should not force users to rewrite their own code.
- **Major release** Signify significant changes that are no longer backwards compatible. Features may be removed or changes substantially.

```
// Initial Release
1.0.0

// Patch Release
1.0.1
```

## `git tag`

- `git tag`: view all the tags in the current repository.
- `git tag -l "*v17*"`:
    - search for tags that match a particular pattern by using `git tag -l` and the passing in a *wildcard pattern*.
    - E.g., `git tag -l "*v17*"` prints a list of tags that include "v17" in their name.
- `git checkout <tag>`:
    - view the state of a repo at a particular tag.
    - goes into detached HEAD.
- `git tag <tag_name>`:
    - creates a lightweight tag.
    - By default, Git will create the tag referring to the commit that HEAD is referencing.
- `git tag -a <tag_name>`:
    - creates an annotated tag.
    - Git opens your default text editor and prompts for additional information.
    - Similar to git commit, can use `-m` to pass a message directly and forgo the opening of the text editor.
- `git tag <tag_name> <commit_hash>`
    - tagging an older commit by providing the commit hash.
- `git tag -f <tag_name>`:
    - If we try to reuse a tag that is already referring to a commit, Git throws a "fatal" message.
    - Use the `-f` option to force the tag through.
- `git tag -d <tag_name>`: delete a tag.
- `git push <remote> <tag_name>`
    - Push a single tag to the remote server.
- `git push --tags` or `git push <remote> --tags`:
    - Push up all of the tags to the remote server that are not already there.