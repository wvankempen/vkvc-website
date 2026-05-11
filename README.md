# vankempenventures.com

The Van Kempen Ventures & Consultancy website. A single self-contained HTML file, no build step.

## Files

| File | Purpose |
|---|---|
| `index.html` | The one-page site. All CSS is inline at the top. |
| `favicon.svg` | Browser tab icon (vector). |
| `favicon.png` | PNG fallback for the favicon. |

## Editing

Open `index.html` in any editor. Brand tokens live under `:root` near the top of the `<style>` block, so the palette and type can be tuned in one place:

- `--ink` — primary
- `--bone` — surface
- `--brass` — accent (use sparingly)
- `--slate` — secondary text
- `--hairline` — rules

The site is responsive down to ~360px and respects `prefers-reduced-motion`.

## Local preview

Any static server will do. Two common options:

```bash
# Python
python -m http.server 8000

# Node (no install)
npx --yes live-server --port=5174
```

Then open http://localhost:5174 (or whichever port you chose).

## Deploying

Drop `index.html` and the favicons on any static host: GitHub Pages, Netlify, Vercel, Cloudflare Pages. No build required.
