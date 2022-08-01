# Git Tutorial

## first install git in the computer

```
Installing on Linux
$ sudo dnf install git-all
```

Installing on windows follow [install-git-windows](https://phoenixnap.com/kb/how-to-install-git-windows 'The best search engine').

---

# Git Commands

create version
Git will start tracking all changes in the current folder

```
git init
```

Show all changes since the previous commit

```
git status
```

Pick changes to go into next commit

```
git add <file|folder>
```

Pick individual file

```
git add filename
```

Pick all files (in folder command line is running in)

```
git add .
```

Configure Name & Email for Commits<br>
username

```
git config --global user.name "Your Name"
```

Email

```
git config --global user.email "email@example.com"
```

Creates a commit with a message attached

```
git commit -m "message"
```

Update previous commit instead of creating new one

```
git commit -m "message" --amend
```

View the commit history

```
git log
```

Show all commits (not just current branch)

```
git log --all
```

Show branching visually in the command line

```
git log --all --graph
```

fix uncommited mistakes or staging. you add but not commited , cancel added file or folder

```
git reset <file|folder>
git reset file
git reset folder/
git reset .
```

fix commited mistake

```
don't forget to fill this command
```

## Viewing Previous Commits

```
git checkout <commit_hash|branch_name>
```

### `master`

1. You can `git checkout branch`
2. Always points to `latest` commit
   on the branch.

### `HEAD` : indicates which commit you are currently viewing

## Restoring to a Previous Commit

Restore the contents of files back to a
previous commit

```
git checkout <hash|branch> <file|folder>
```

Restore a file

```
git checkout <hash|branch> file
```

Restore all files in folder (& subfolders)

```
git checkout <hash|branch> folder/
```

Restore all files in project

```
git checkout <hash|branch> .
```

## Other Features of Git

Creates an alias (a shortcut)

```
git config --global alias.shortcut <command>
```

### example

```
git config --global alias.s "status" == git s
```

1. git s = git status
