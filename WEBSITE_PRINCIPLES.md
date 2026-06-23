# Website Architecture

- **Hugo** — fast static site generator; single binary, no runtime dependencies
- **Standalone theme** — no external module dependencies; all layouts and CSS are in-repo for full control
- **Warm earth-tone palette** — professional, grounded aesthetic; avoids clinical look
- **Dense citation lists** — academic scanability; tab-filtered client-side with vanilla JS
- **Accordion research areas** — organize related works on homepage; avoid flat publication dumps
- **Stable URLs** — `/publication/slug/` permalinks; academic citations persist
- **Vanilla JS** — no framework; degrades gracefully if JS disabled
- **GitHub Pages + Actions** — automated deployment on every push to main
- **CSS architecture** — single `custom.css` file; CSS custom properties for theming
- **Footer credit** — "Created using GaryKing.org/mysite" in persistent footer
