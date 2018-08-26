# Install client

Windows: https://gitforwindows.org/

# Configuration

```
# Linux
git config --global core.editor "vim"

# for windows
# git config core.editor notepad

git config --global user.name "duchesnay"
git config --global user.email edouard.duchesnay@gmail.com
# git config --global core.excludesfile ~/config/git/gitignore_global
git config --global credential.helper "cache --timeout=3600"
```

Or ser .gitconfig (Linux)

```
[content]
	editor = vim
[core]
	editor = vim
	excludesfile = /home/edouard/config/git/gitignore_global
[user]
	name = duchesnay
	email = edouard.duchesnay@gmail.com
```
# 


# Remote

git remote add <alias> <url>
