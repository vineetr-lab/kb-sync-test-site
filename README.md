# kb-sync test site

A deliberately boring static site for exercising knowledge-base **website import and sync**.

Published with GitHub Pages. Four pages, no sitemap (see `robots.txt` for why).

## Using it

1. Import some or all of the four pages into a KB.
2. Sync once — everything reports `unchanged`, baselines are stamped, nothing uploads.
3. **Edit `pricing.html`** in the GitHub UI, commit, wait ~30s for the deploy.
4. Sync again — that one page reports `updatedContent`; the others stay `unchanged`.
5. **Delete `changelog.html`** and sync — it reports `removed` (the page 404s).

`security.html` is the control: it should never change.
