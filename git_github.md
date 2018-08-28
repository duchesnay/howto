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

# Classic workflow

See cheatsheet: https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet

```
git pull
echo toto > fic1.txt
git add fic1.txt
git commit -am "fic1"
git push

echo titi >> fic1.txt
```
Uncommited changes

```
git diff
diff --git a/fic1.txt b/fic1.txt
index fbcf12d..14bc6c5 100644
--- a/fic1.txt
+++ b/fic1.txt
@@ -1 +1,2 @@
 toto
+titi

Or

```
git status
```

Commited changes

```
git diff --cached

[...]
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   fic1.txt
```

# Basic commands

Sources:

- 

- Tuto (in french): http://www.alexgirard.com/git-book/
