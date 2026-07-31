# Longevity Compass — deploy bundle

## Structure
- `wrangler.toml`  → tells Cloudflare to serve the site as static assets
- `public/`        → everything that gets served
  - `index.html`   → the site (loads at your domain root)
  - logo + favicon files

## Deploy (Cloudflare, via GitHub)
1. Put these files at the root of your repo, keeping this exact structure.
2. Commit and push.
3. Cloudflare build settings: Root directory `/`, Build command `None`,
   Deploy command `npx wrangler deploy`.

## Edit later
- Swap partner names, prices, and tracking links inside `public/index.html`
  (each card's `<a class="visit" href="...">`). Keep `rel="sponsored nofollow"`.
