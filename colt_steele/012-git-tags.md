# Git Tags: Marking Important Moments in History

## Git Tags

- Tags are pointers that refer to particular points in Git history.
- Often used to mark version releases in projects (v4.1.0, v4.1.1, etc.)
- Tags are like branch references that do not change.
    - Once a tag is created, it always refers to the same commit.
    - Just a label for a commit.

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