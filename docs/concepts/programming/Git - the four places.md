

## The four places

**Working directory, staging area, local repo, remote repo.** The first three live on my computer’s disk: the working directory is my project folder, and the staging area and local repo both live inside the hidden `.git` folder. The remote repo lives on GitHub’s servers.

## Commands that move changes between them

Working directory  --git add-->  Staging area  --git commit-->  Local repo  --git push-->  GitHub

## What a commit (snapshot) is

A commit is a permanent snapshot of the entire project: the last commit plus my staged changes. It records an ID, author, date, message, and the commit before it.

## What staging is for

Staging lets me choose what goes into each commit, so unfinished or unneeded changes can wait. Example: stage a finished bug note but leave a half-written concept note out. It’s also a chance to review with `git status` before committing.

## Where the repo actually lives

The `.git` folder is the repository: it stores commits, the staging area, and settings like the `origin` link to GitHub. Everything else in the repo folder is my working files. Obsidian and Git aren’t connected directly; the vault (`docs/`) sits inside the repo folder, and Git tracks everything inside that folder, so every note Obsidian saves is tracked like any other file.

## How Git finds the repo

Git will check the current and parent folder to find a git folder and cross compare files you have and they have.