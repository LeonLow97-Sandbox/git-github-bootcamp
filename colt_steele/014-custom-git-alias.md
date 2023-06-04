# Writing Custom Git Aliases

- Useful for writing custom git commands locally.
- [Git Alias GitHub Repo](https://github.com/GitAlias/gitalias)
- [Must Have Git Aliases Blog Post](https://www.durdn.com/blog/2012/11/22/must-have-git-aliases-advanced-examples/)
- [The Ultimate Git Alias Setup](https://gist.github.com/mwhite/6887990)

## Global Git Config

- Git looks for the global config file at `~/.gitconfig` or `~/.config/git/config`.
- Any configuration variables that we change in the file will be applied across al Git repos.
- Can also alter configuration variables from the command line if preferred.

## Adding Aliases

- `git config --global --edit`: to open the global git config file.

``` 
[alias]
	s = status
	l = log
	a = add .
	cm = commit -m 
```

## Adding Aliases from Command Line

- `git config --global alias.showbranches branch`
    - alias `git showbranches` equates to `git branch`