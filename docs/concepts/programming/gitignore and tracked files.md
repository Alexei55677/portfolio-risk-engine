## .gitignore pattern rules

| Pattern | Matches | Example use |
|---|---|---|
| `name.ext` | Any file with that name, in any folder | `scratch.txt` |
| `folder/` | That folder and everything inside it | `data/` |
| `*.ext` | Every file ending in that extension (`*` = any characters) | `*.csv` |
| `path/to/name*` | Anything in that specific folder starting with `name` | `docs/.obsidian/workspace*` |
| `/name.ext` | That file in the repo root only, not in subfolders | `/notes.txt` |
| `!name.ext` | Un-ignores a file that an earlier rule ignored | `!keep.csv` after `*.csv` |
| `# text` | A comment; Git skips the line | `# Obsidian settings` |

**Reminder:** rules only apply to untracked files. If a file is already tracked, run `git rm --cached <file>` and commit.