# coltwarren.com

Personal website for Colt Warren, deployed on Cloudflare Workers using Static Assets.

## Production

Primary domain:

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