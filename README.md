# parthpatel.si

Personal portfolio of Parth Patel. Static site (HTML + CSS), no build step, hosted on GitHub Pages.

## Edit content
Everything lives in `index.html`. Search for `[` to find the remaining placeholders.

## Deploy (GitHub Pages)
1. Push this repo to GitHub (public repo, `main` branch).
2. Repo → Settings → Pages → Source: "Deploy from a branch" → `main` / `(root)` → Save.
3. Custom domain: `parthpatel.si` (already set by the `CNAME` file). Tick "Enforce HTTPS" once the certificate is issued.

## DNS (Hostinger → Domains → parthpatel.si → DNS / Nameservers)
Delete any existing A / AAAA records for `@` and the default `www` record, then add:

| Type  | Name | Value                  |
|-------|------|------------------------|
| A     | @    | 185.199.108.153        |
| A     | @    | 185.199.109.153        |
| A     | @    | 185.199.110.153        |
| A     | @    | 185.199.111.153        |
| CNAME | www  | <github-username>.github.io |

DNS can take from a few minutes up to 24 hours to propagate.
