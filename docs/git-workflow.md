# Git workflow

A clean history shows employers how you work. These habits cost nothing and are easy to explain in an interview.

## One-time setup

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global init.defaultBranch main
```

## The daily loop

```bash
git status                      # what changed?
git switch -c feat/booking-form   # a new branch for one piece of work
# ...edit files, run the tests...
git add projects/booking-app/src/app/booking-form
git commit -m "feat: add booking form validation"
git push -u origin feat/booking-form   # first push of a branch
```

Then open a pull request on GitHub, read your own diff, and merge it. Reviewing your own pull request is a
good habit: you often spot mistakes before anyone else does.

## Commit messages

Format: `type: short summary in the imperative`, 72 characters or fewer.

| Type | Use it for |
|---|---|
| `feat` | something new |
| `fix` | a bug fix |
| `docs` | README or other documentation |
| `test` | adding or changing tests |
| `refactor` | restructuring without changing behaviour |
| `chore` | tooling, config, dependencies |

| Weak | Better |
|---|---|
| `made it to index.html` | `fix: point the build output to index.html` |
| `add to github` | `chore: add project to GitHub` |
| `changes` | `feat: add date picker to the booking form` |

## Habits

- **Small commits, one purpose each.** If you need the word "and" in the message, make two commits.
- **Commit working code.** Run the tests first.
- **Never commit** `node_modules/`, `.env` files, passwords or keys. They belong in `.gitignore`.
- **Do not rewrite history** on anything you have already pushed. Fix forward with a new commit.
- **Write the README as you go**, not at the end.

## Useful commands

| Command | What it does |
|---|---|
| `git status` | Show what is changed and staged |
| `git diff` | Show unstaged changes |
| `git log --oneline -10` | Last 10 commits, one line each |
| `git switch main` | Go back to the main branch |
| `git restore <file>` | Throw away unstaged changes to a file (cannot be undone) |
| `git stash` / `git stash pop` | Put changes aside, then bring them back |

## Putting this repository on GitHub (first time)

1. On github.com, create a new **empty** repository named `frontend-portfolio` (do not tick "Add a README").
2. In this folder:

```bash
git remote add origin https://github.com/sirivalli75/frontend-portfolio.git
git push -u origin main
```

3. In the repository's About box, add a one-line description and your topics (`angular`, `typescript`, `portfolio`).
4. Pin it on your GitHub profile.
