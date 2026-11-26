# Portfolio checklist

What a hiring manager sees in about 30 seconds: your GitHub profile, a pinned repository, its README and its commits.
Use this list on every project you want to show.

## For each project you want to show

- [ ] README written from the template: what it is, screenshot, live link, how to run it
- [ ] The app is deployed, and the live link works (check it in a private window)
- [ ] A short "what I learned and decisions I made" section
- [ ] Tests exist and `npm test` passes; a GitHub Actions workflow runs them
- [ ] No `node_modules/`, `dist/`, `.env` files or keys in the repository
- [ ] A clear repository name and a one-line description in GitHub's About box
- [ ] Topics added (`angular`, `typescript`, ...)
- [ ] Mobile layout works, and the accessibility score in Lighthouse is high

## Secrets check (do this before anything goes public)

- A Supabase **anon / publishable** key is designed to be public. The **service-role** key never is.
- Search each project for `service_role`, `secret`, `password` and `.env`.
- If a secret was ever committed, rotate it (create a new one and revoke the old). Deleting it from the latest
  commit does not remove it from history.

## Client work

- Ask the client before listing the project, and list only what they are happy to show.
- Link to the live site and describe your role. Do not copy client code into this repository.
- Keep learning and practice files out of the client's repository.

## Your GitHub profile

- [ ] Profile photo and a short bio
- [ ] Pin 3 to 6 repositories: this portfolio, your best two projects
- [ ] Optional: a profile README (a repository named exactly like your username, here `sirivalli75`)
- [ ] Contribution graph: a few commits most weeks looks better than one burst
