# Basic Git and GitHub Cheat Sheet

## Learning Resources

| Resource | Channel | Language |
| --- | --- | --- |
| [Learn Git and Github (playlist)](https://youtube.com/playlist?list=PLDoPjvoNmBAw4eOj58MZPakHjaO3frVMF) | Elzero Web School | Arabic |
| [Learn Git & GitHub in One Hour Crash Course](https://www.youtube.com/watch?v=fDkR0TDR9dI) | Ghareeb Elshaikh | Arabic |
| [Learn Git and GitHub in 1 Hour!](https://www.youtube.com/watch?v=lLoJHifWTRw) | Alex The Analyst | English |
| [Git and GitHub Tutorial for Beginners](https://www.youtube.com/watch?v=tRZGeaHPoaw) | Kevin Stratvert | English |
| [Git & GitHub Crash Course for Beginners (2026)](https://www.youtube.com/watch?v=mAFoROnOfHs) | freeCodeCamp.org | English |

Replace anything in `<>` with your own value.

## Set up once & Start

| Command | What it does |
| --- | --- |
| `git config --global user.name "<name>"` | Set the name on your commits |
| `git config --global user.email "<email>"` | Set the email on your commits |
| `git config --global init.defaultBranch main` | Name the first branch `main` in new repos |
| `git config --list` | Show current settings |
| `git init` | Turn the current folder into a repository |
| `git clone <url>` | Copy an existing repository |
| `git help <command>` | Open the manual for a command |

**Explanation:** Set your name and email once, then create a new project or copy an existing one.

## Save your work

| Command | What it does |
| --- | --- |
| `git status` | Show changed, staged and untracked files |
| `git add <file>` | Stage a file (`git add .` stages the current folder) |
| `git add -p` | Stage changes piece by piece |
| `git add -A` | Stage all changes, including deletions |
| `git commit -m "<message>"` | Commit/save what is staged |
| `git commit -am "<message>"` | Stage tracked files and commit (skips new files) |
| `git log` | View full history |
| `git log --oneline` | View history, one line per commit |
| `git log -p <file>` | History of one file, with changes |
| `git diff` | View unstaged changes |
| `git diff --staged` | Show staged changes |
| `git show <commit>` | Show one commit |
| `git blame <file>` | Show who last changed each line |
| `git mv <old> <new>` | Rename a file and stage the rename |
| `git rm <file>` | Delete a file and stage the deletion |

**Explanation:** Choose your changes (`add`), save them (`commit`), and review changes and history.

## Branches

| Command | What it does |
| --- | --- |
| `git branch` | List branches |
| `git checkout` | Show changed files and tracking status |
| `git checkout <branch>` | Move to a branch |
| `git switch <branch>` | Move to a branch |
| `git switch -c <branch>` | Create a branch and move to it |
| `git merge <branch>` | Merge a branch into the current one |
| `git branch -d <branch>` | Delete a merged branch |

**Explanation:** A branch is a separate space to try out changes. Merge it when the work is ready.

## GitHub

| Command | What it does |
| --- | --- |
| `git remote -v` | List remotes and their URLs |
| `git remote add origin <url>` | Connect a local repo to GitHub |
| `git remote set-url origin <url>` | Change a remote's URL |
| `git fetch` | Download changes without merging them |
| `git pull` | Get the latest changes |
| `git pull --rebase` | Fetch, then replay your commits on top |
| `git push -u origin <branch>` | First push of a new branch, and track it |
| `git push` | Upload new commits to the tracked branch |
| `git push origin --delete <branch>` | Delete a remote branch |

To open a pull request, push your branch, then choose **Compare & pull request** on GitHub.

**Explanation:** Connect your project to GitHub, upload your changes (`push`), and download changes from others (`pull`).

## Undo

| Command | What it does |
| --- | --- |
| `git restore --staged <file>` | Unstage a file |
| `git restore <file>` | Discard unstaged edits (cannot be undone) |
| `git revert <commit>` | Reverse a commit with a new commit |

**Explanation:** Unstage a file, discard its edits, or reverse an earlier commit.

## Notes

- Run `git status` before each commit to check what you are saving.
- Write short, clear commit messages.
- Run `git pull` before you start working.
- Work on a separate branch instead of `main`.
- List files you don't want to track in `.gitignore`.
- Never push passwords or API keys to GitHub.
- To resolve a merge conflict: edit the file, run `git add <file>`, then `git commit`.
