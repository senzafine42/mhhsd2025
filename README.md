# Mile High Heli Showdown (MHHS)

Official website for the Mile High Heli Showdown event.

## Live Site
- https://milehighhelishowdown.com/

## What’s in this repo
Static HTML/CSS site:
- `index.html` – homepage / schedule
- `location.html` – field details
- `register.html` – registration info
- `contact.html` – contact info
- `style.css` – styling
- `img/` – site images

## Local Development
Just open `index.html` in a browser, or run a tiny web server:

```bash
# Python
python -m http.server 8080
# then open http://localhost:8080
```

## Deployment

- Hosting: <S3 static website / Netlify / etc.>
- CDN: <CloudFront / Cloudflare / None>
- DNS: <Route53 / Cloudflare / Other>

Deployment notes:
- Static site deployment
- No server-side rendering
- No backend services

## Performance

Performance optimizations tracked intentionally:

- [ ] Images converted to WebP/AVIF and resized
- [ ] Cache-Control headers set for static assets
- [ ] Brotli/Gzip compression enabled
- [ ] Lighthouse score recorded per release

## Security

Baseline security expectations:

- [ ] Web access to `/.git/*` blocked
- [ ] Security headers enabled (HSTS, CSP, etc.)
- [ ] HTTPS enforced site-wide
