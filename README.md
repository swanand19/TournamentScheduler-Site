# KickCricket — website

The public site for the app: what it is, the privacy policy and how to delete an account.
Plain HTML and CSS, no build step. Served by GitHub Pages.

- `index.html` — the home page
- `privacy.html` — privacy policy (Google Play and Meta link here)
- `delete-account.html` — how to delete an account (Google Play links here)
- `styles.css`, `mark.svg` — the look and the icon
- `.nojekyll` — tells GitHub Pages to serve the files as they are

## Publish

1. Push this folder to a **public** GitHub repo.
2. Repo → Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)` → Save.
3. After a minute it's at `https://<username>.github.io/<repo>/`
   (or `https://<username>.github.io/` if the repo is named `<username>.github.io`).

Links between pages are relative, so either address works.

## Keep it true

The privacy and delete pages are copies of the web app's `src/legal/LegalPage.jsx`. When a feature changes what
the app keeps or who sees it, change both, and the "Last updated" date.
