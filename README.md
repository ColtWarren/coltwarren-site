# coltwarren.com

Personal website for Colt Warren, deployed on Cloudflare Workers using Static Assets.

## Production

Primary site:

https://coltwarren.com

`www.coltwarren.com` permanently redirects to the apex domain while preserving paths and query strings.

## Architecture

```text
GitHub
ColtWarren/coltwarren-site
        ↓
Wrangler
        ↓
Cloudflare Workers
        ↓
Workers Static Assets
        ↓
coltwarren.com
```

## Project Structure

```text
coltwarren-site/
├── public/
│   └── index.html
├── README.md
├── package.json
└── wrangler.jsonc
```

## Local Development

```bash
pnpm install
pnpm dev
```

## Deployment

```bash
pnpm deploy
```

The production custom domain is configured in `wrangler.jsonc`.

## Stack

- HTML
- CSS
- Cloudflare Workers
- Workers Static Assets
- Wrangler
- pnpm
- Git
- GitHub

## Repository

https://github.com/ColtWarren/coltwarren-site

## Design Principle

Keep the public website simple and independently deployable.

Cloudflare OS experimentation and future personal Cloudflare OS infrastructure remain separate from this repository.