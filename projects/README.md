# Projects

Each project lives in its own folder here, named for what it is (`booking-app`, `recipe-finder`, not `test1`).

## Starting a project

```bash
cd projects
# Angular:
npx @angular/cli@latest new project-name
# or Vite (React, vanilla TypeScript, ...):
npm create vite@latest project-name
```

Then:

1. Replace the generated README with one written from [the template](../docs/project-readme-template.md).
2. Make sure the project's own `.gitignore` keeps `node_modules/` and `dist/` out of git.
3. Commit early, in small steps ([git workflow](../docs/git-workflow.md)).
4. Add a row to the "Featured projects" table in the main README when it is worth showing.

## One repository or many?

You can build here, one folder per project, or give your best projects their own repositories and link them from the
main README. Many employers like a standalone repository for a flagship project. Either way, the same rules apply:
a real README, a live demo, tests, and no secrets in git.

## Rules

- Never commit `.env` files, keys or passwords.
- Never put client or freelance work in this repository. Link to the live site instead.
