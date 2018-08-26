# Install client

Windows: https://gitforwindows.org/

# Configuration

```
# Linux
git config --global core.editor "vim"

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

## Credential

### Windows

Use the Git credential helper on Windows, can be obtained here:
https://github.com/Microsoft/Git-Credential-Manager-for-Windows

### Linux

Generate key

```
ssh-keygen
```

Copy `./ssh/id_rsa.pub` into github


# Clone Repo

```
git clone git@github.com:duchesnay/test.git
```

# Remote

```
git remote -v
```

Adding Remote Repositories

```
git remote add <alias> <url>
```

# Fetching and Pulling / Pushing from Your Remotes

git fetch [remote-name]
git push [remote-name] [branch-name]
git remote add <alias> <url>

# Basic commands

Sources:

- cheatsheet: https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet

- Tuto (in french): http://www.alexgirard.com/git-book/
