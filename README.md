# marcamil30.github.io

Personal site. Plain HTML, CSS and a few lines of JS — no framework, no build step.

```
index.html          # all content lives here
css/style.css       # design tokens + layout (dark/light via [data-theme])
js/main.js          # theme toggle, remembers choice in localStorage
assets/             # CV pdf
```

## Run locally

```bash
python3 -m http.server 4173
```

Then open http://localhost:4173

## Deploy

Pushing to `main` publishes automatically via GitHub Pages
(Settings → Pages → Source: Deploy from a branch → `main` / root).

## Editing

Content is in `index.html`, section by section. Colours are CSS custom
properties at the top of `css/style.css` — change `--accent` to retheme.
