# Git commands

| Command | What it does | Example |
|---|---|---|
| `git clone <url>` | Copies a GitHub repo into a new folder in the current directory: working files, `.git` with full history, and an `origin` link back to GitHub | From `C:\Dev`: `git clone https://github.com/Alexei55677/portfolio-risk-engine.git` |
| `git status` | Shows whether commits match GitHub, and whether files have unstaged, staged, or untracked changes | Start and end of every session; aim for *up to date* and *working tree clean* |
| `git add <file>` / `git add .` | Stages a file as it is right now, or with `.` every changed file in the current folder and below | `git add .` from the repo root |
| `git commit -m "msg"` | Saves everything staged as a permanent snapshot in the local repo, with ID, author, and message | `git commit -m "Add title to index"` |
| `git push` | Uploads all local commits GitHub doesn't have; uncommitted changes are not sent | `git push`, then look for `main -> main` |
| `git config --global user.name/user.email` | Sets the name and email stamped on every commit; `--global` = all repos on this computer | `git config --global user.name "Alexei Kraytman"` |
| `git rm --cached <file>` | Stops tracking a file but keeps it on disk; commit afterward. File stays in old commits | `git rm --cached docs/.obsidian/workspace.json` |
| `git check-ignore -v <file>` | Shows which `.gitignore` file, line, and rule ignores a file. Skips tracked/staged files unless `--no-index` | `git check-ignore -v --no-index docs/.obsidian/workspace.json` |
| `git diff <file>` | Shows unstaged changes vs last commit (`-` removed, `+` added). `--staged` shows staged changes | `git diff .gitignore` |
| `git restore <file>` | Discards unstaged edits, resetting to last commit. **Permanent.** `--staged` unstages instead, keeping edits | `git restore --staged README.md` |
| `git log --oneline` | Lists commits newest first; `HEAD` = where you are, `origin/main` = what GitHub has | `git log --oneline` |
| `git remote -v` | Shows linked remotes and their URLs (`origin` = GitHub) | `git remote -v` |

