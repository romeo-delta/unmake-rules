# unmake-rules

Live `toggles.json` and `themes.json` for the [unmake](https://github.com/romeo-delta/unmake)
iOS app, served via GitHub Pages so a broken selector can be fixed without an
App Store review.

This repo is a deploy target, not where you edit rules by hand — the source
of truth and validation live in the main `unmake` repo's `rules/` directory.
Pushing to `main` there (via `.github/workflows/deploy-rules.yml`) validates
the JSON with the same `RuleValidator` the app runs, then syncs the validated
files here.

Served at:
- `https://romeo-delta.github.io/unmake-rules/toggles.json`
- `https://romeo-delta.github.io/unmake-rules/themes.json`
