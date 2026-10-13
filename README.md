# Xiaowu Wu - personal portfolio

A concise, responsive English portfolio in plain HTML and CSS, with optional JavaScript. No build step or external runtime dependencies.

## Local preview

Open `dist/index.html` directly, or run from this folder:

    python -m http.server 8000 --bind 127.0.0.1 --directory dist

Then visit http://127.0.0.1:8000.

## Content

- About: one-sentence background and a visual toolkit.
- Projects: DND Map screenshot and link to the interactive demo; other projects can be added later.
- Connect: email, LinkedIn and GitHub.

Detailed education and experience, resume download links, and hero buttons have been removed. The original resume file is retained locally but is not linked from the page.

## Editing

- `dist/index.html`: content, inline tool icons and project entries.
- `dist/assets/DND-Map-Project.png`: the supplied, uncropped DND Map screenshot. Its project card links to https://mikawu73.github.io/DND-Map-Demo/.
- `dist/styles.css`: visual design and mobile layout.
- `dist/assets/tools/`: source SVGs and icon attribution/license.

The hero illustration is decorative, not measured data. No invented project outcomes or proficiency ratings are displayed.

## GitHub Pages

The site uses GitHub Pages' existing branch deployment: `main`, `/(root)`.
The root `index.html` is a small Jekyll entry point that includes `dist/index.html`
and adjusts its stylesheet, script and asset paths. It disables the default theme
layout, so the project URL shows the portfolio instead of this README.

Keep editing `dist/index.html` and its assets. The root entry point reuses that
content on every Pages build; no second copy of the page needs to be maintained.
Local previews and Sites deployments continue to serve `dist/` directly.
