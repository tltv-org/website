# tltv-org-website

Landing page for [timelooptv.org](https://timelooptv.org) — a federation protocol for open television channels.

## Structure

```
index.html        — landing page
manifesto.html    — manifesto page
license.html      — MIT license page
style.css         — all styles
favicon.svg       — mark favicon (dark mode aware)
tltv-lockup.svg   — mark + wordmark for hero
og-image.png      — 1200x630 OG social preview
sitemap.xml       — sitemap
Dockerfile        — nginx container for local preview
```

No JavaScript. No build step. No frameworks.

## Local preview

```
docker build -t tltv-site . && docker run -d -p 8080:80 tltv-site
```

Then open `http://localhost:8080`.

## Deploy

Deployed to Cloudflare Pages from GitHub mirror. Push to `github/main` triggers a deploy.

- Build command: *(none)*
- Output directory: `/`
- Domain: timelooptv.org

## License

MIT -- see [LICENSE](LICENSE).
