# marcamil30.github.io

Personal site. Plain HTML, CSS and ~20 lines of JS — no framework, no build step.

```
index.html       # all content, section by section
css/style.css    # greyscale tokens at the top, then layout
js/main.js       # light/dark toggle, remembers the choice
assets/img/      # photo goes here
```

## Add your photo

Drop a square image at `assets/img/marc.jpg`. Until then the site shows an
"MA" monogram — nothing breaks either way. Roughly 400×400 is plenty.

## Swap a project thumbnail for a real figure

Each entry's figure is an inline `<svg>` inside `<div class="item__fig">`.
Replace the whole `<svg>…</svg>` with:

```html
<img src="assets/img/my-figure.png" alt="">
```

## Run locally

```bash
python3 -m http.server 4173
```

Then open http://localhost:4173

## Deploy

Push to `main`; GitHub Pages serves it
(Settings → Pages → Source: Deploy from a branch → `main` / root).

## Retheme

Everything is greyscale custom properties at the top of `css/style.css` —
`:root` for light, `html[data-theme="dark"]` for dark.
