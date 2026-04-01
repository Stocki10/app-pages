# app-pages

Reusable GitHub Pages site for App Store support, marketing, privacy, and legal URLs.

## Purpose

This repository is a multi-app static site intended for GitHub Pages project hosting.

Current URL pattern:

- `/` publisher landing page
- `/apps/<app-slug>/` app marketing page
- `/apps/<app-slug>/support/` support page
- `/apps/<app-slug>/privacy/` privacy policy
- `/apps/<app-slug>/legal/` copyright and legal page

## Current app

- `dartscorer`

## Folder structure

```text
.
|-- index.html
|-- styles.css
|-- .nojekyll
`-- apps
    `-- dartscorer
        |-- index.html
        |-- support
        |   `-- index.html
        |-- privacy
        |   `-- index.html
        `-- legal
            `-- index.html
```

## How to add a new app

1. Copy `apps/dartscorer/` to `apps/<new-app-slug>/`.
2. Replace the app-specific content in the copied files:
   - app name
   - support email
   - developer or publisher name
   - app summary and features
   - privacy details
   - legal notice
   - App Store link if available
3. Add the new app card to `index.html`.
4. Commit and push to the `main` branch.

## App-specific values to replace

- `Just a Darts Scorer`
- `dartscorer`
- `Stocki`
- `l.stockmann.10@gmail.com`
- feature list
- privacy details
- legal/copyright wording

## GitHub Pages

Recommended setup:

- Repository: `Stocki10/app-pages`
- Visibility: public
- Branch: `main`
- Folder: `/ (root)`

This site is plain HTML and CSS only. No build step is required.
