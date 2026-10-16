# Reach Point Lab website

Source for reachpointlab.com. Plain HTML, CSS and JavaScript, no build step and nothing to install.

## Pages

| Path | What it is |
| --- | --- |
| `index.html` | Home page: hero, the three apps, philosophy. |
| `privacy/stool.html`, `privacy/fast.html`, `privacy/lucid.html` | App privacy policies, served as `/privacy/stool` etc. (Vercel `cleanUrls`). These URLs are referenced by the apps, so do not rename them. |
| `assets/site.css`, `assets/site.js` | Shared styles and behavior, including the animated background and the light/dark toggle. |
| `images/` | App icons (512px) and the logo. |

## Keep in sync

The header and footer markup is copied into `index.html` and each privacy page, because there is no build step.
If you change the nav or footer, change it in all four files. `assets/site.css` and `assets/site.js` are also
adapted from the Reach Point Capital site (`rpc-website`), so design changes usually belong in both repos.

## Run it locally

Any static server that understands clean URLs works, e.g. `npx vercel dev`, or open `index.html` directly for a
quick look (the privacy links need a server).

## Deploying

Pushing to `main` deploys to production on Vercel; other branches get a preview URL. The site as it was before the
October 2026 redesign is kept as the git tag `archive/old-site-2026-10-15`.

News and announcements live on the main site's newsroom: https://reachpointcapital.com/newsroom/
