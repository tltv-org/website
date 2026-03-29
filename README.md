# tltv-org-website

Landing page for [timelooptv.org](https://timelooptv.org) — a federation protocol for open television channels.

## Structure

```
index.html    — single-page site
style.css     — all styles
Dockerfile    — nginx container for local preview
```

No JavaScript. No build step. No frameworks.

## Local preview

```
docker build -t tltv-site . && docker run -d -p 8080:80 tltv-site
```

Then open `http://localhost:8080`.

## Deploy

Deployed to Cloudflare Pages. Push to `main` triggers a deploy.

- Build command: *(none)*
- Output directory: `/`

## License

MIT -- see [LICENSE](LICENSE).
