# ambiquality-web

Static GitHub Pages site for **ambiquality.org**, announcing that the Ambiquality IEQ
monitoring platform has been taken offline for running-cost reasons.

## Deploying to GitHub Pages

1. Push this to a GitHub repository named `ambiquality-web` (or similar).
2. Repository → **Settings → Pages**.
3. Under **Build and deployment → Source**, select **Deploy from a branch**.
4. Choose the `main` branch and **/(root)** directory, then save.
5. The site will be published at `https://<owner>.github.io/<repo>/`.

## Custom domain (ambiquality.org)

1. Add a `CNAME` file to the repo root containing `ambiquality.org` (already present here).
2. In Settings → Pages → **Custom domain**, enter `ambiquality.org` and save.
3. Point your DNS records at GitHub Pages:
   - `A` record → `185.199.108.153`
   - `A` record → `185.199.109.153`
   - `A` record → `185.199.110.153`
   - `A` record → `185.199.111.153`
   - `CNAME` `www` → `<owner>.github.io`
4. Re-point the app's existing DNS records (currently `ambiquality.org`) to the same targets.
