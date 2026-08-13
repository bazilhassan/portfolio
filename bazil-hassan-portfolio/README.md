# Bazil Hassan — Portfolio

Production-ready static portfolio for `bazilhassan.com`.

## Structure

```text
portfolio/
├── public/
│   ├── index.html
│   ├── robots.txt
│   ├── sitemap.xml
│   └── assets/
│       ├── Bazil-Hassan-Resume.pdf
│       └── opic-camera-ui.webp
├── wrangler.jsonc
└── .gitignore
```

## Cloudflare Workers deployment

This matches your current GitHub → Cloudflare Workers Static Assets setup.

After replacing your repository files with this package, use:

```bash
npx wrangler deploy
```

The `wrangler.jsonc` now contains:
- Worker name: `portfolio`
- compatibility date
- static asset directory: `./public`

So you no longer need `--assets .` and Cloudflare will not upload `.git` or other repository files as website assets.

## Custom domain

After the Worker deploy succeeds:

Cloudflare → Workers & Pages → `portfolio` → Settings / Domains & Routes → Add → Custom Domain → `bazilhassan.com`

## Information already wired in

- Domain: https://bazilhassan.com
- Professional email: bazil@bazilhassan.com
- LinkedIn: https://www.linkedin.com/in/bazil-hassan/
- GitHub: https://github.com/bazilhassan
- OPIC3D App Store
- Sibme App Store
- Lujo App Store
- Weeks App Store
- Tap for Joy App Store
- Verideal App Store
- Current resume PDF

## Still worth adding later

Real, approved product screenshots for:
- Sibme
- Mr. Rebounder
- Hyphen
- Lujo

The included OPIC visual is the camera UI concept extracted from your existing OPIC camera specification. It is labeled as a concept in the portfolio, not presented as a shipped screenshot.

If you provide approved screenshots later, compress them to WebP/AVIF and replace the project visual blocks without changing the page structure.
