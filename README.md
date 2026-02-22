# Walker's TOE — Static site

Files added:

- `index.html` — Main theory page with transcendental background and shimmer divider.
- `breakdown.html` — Break-Down page with sections, sources, and context.
- `gimoire.html` — Link page that opens `https://gimoire.com`.
- `styles.css` — Styles for layout, animated background, and shimmer effects.

- `quickref.html` — Quick Reference: terms and concise definitions used across the site.

To view locally, open `index.html` in your browser (double-click or use your editor's live preview).

Optionally run a simple static server (Python):

```bash
python -m http.server 8000
# then open http://localhost:8000/index.html
```

Cloudflare Wrangler deploy
-------------------------

This repository includes a minimal `wrangler.jsonc` so you can deploy the static files as Cloudflare Worker assets.

Run:

```bash
npx wrangler deploy
```

If you want to specify a different assets directory, edit `wrangler.jsonc` or run:

```bash
npx wrangler deploy --assets=./dist
```

Note: you will need to be authenticated with Cloudflare (via `wrangler login` or env vars) and have a Cloudflare account.
# walkerstoe
Walker's Theory of Everything
