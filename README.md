# petrolpumpsnearme

Static near-me site — **Petrol Pumps Near Me — Find Nearby, Free Map**.

- Live: https://petrolpumpsnearme.pages.dev
- Cloudflare Pages project: `petrolpumpsnearme`
- Sitemap: https://petrolpumpsnearme.pages.dev/sitemap.xml

## Deploy

Static files at the repo root. Two paths:

1. `.github/workflows/deploy.yml` — on push to `main`, needs
   `CLOUDFLARE_API_TOKEN` + `CLOUDFLARE_ACCOUNT_ID` as repo secrets.
2. **Network bridge** — `net-deploy-queue.yml` in `digipincode-india`
   deploys this repo to the `petrolpumpsnearme` Pages project using that repo's
   secrets. Push `deploy-queue/petrolpumpsnearme.json` there to trigger it.

## Rules

- One repo per site. This repo owns only `petrolpumpsnearme`.
- Never copy another site's data or branding here.
- Keep the host in `sitemap.xml` and `robots.txt` correct.
