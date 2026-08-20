# frostclient-site

Marketing site for [FrostClient](https://github.com/QuiteFrosty/FrostClient) — an open-source,
zero-telemetry Minecraft PvP client built on Forge.

Static HTML/CSS/JS. No build step, no dependencies.

## Structure

```
index.html          landing page (hero, features, modules, versions, install, FAQ)
download.html       download + manual install guide + troubleshooting
404.html            not-found page
assets/css/style.css   design tokens and all components
assets/js/main.js      sticky header, mobile nav, copy buttons, scroll reveal
assets/img/            snowflake mark + favicon (SVG)
```

## Running locally

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploying

Pushing to `main` publishes the site through GitHub Pages via
`.github/workflows/pages.yml`. Enable Pages for the repository with
**Settings → Pages → Source: GitHub Actions** once, and the workflow handles the rest.

## Editing

Colours, spacing and type are all CSS custom properties at the top of
`assets/css/style.css` — change them there rather than in individual components.
