# Deploy this site to Cloudflare Pages

This repository is a static website. It does not need a framework, package install, or build step.

## Recommended: connect the GitHub repository

1. Push this repository to your own GitHub account.
2. In Cloudflare, open **Workers & Pages** and choose **Create application**.
3. Choose **Pages**, then **Import an existing Git repository**.
4. Select your GitHub repository and use these settings:

   - Production branch: `main`
   - Build command: `exit 0`
   - Build output directory: `.`
   - Root directory: leave blank

5. Deploy. Cloudflare will provide a `*.pages.dev` address and will redeploy after every push to `main`.

## Optional: custom domain

Open the Pages project, choose **Custom domains**, and add the domain or subdomain you want to use. Do not restore the upstream `CNAME` file; Cloudflare manages the domain in the project settings.

## Where to customize

- Chinese navigation and cards: `cn/index.html`
- English navigation and cards: `en/index.html`
- Chinese and English about pages: `cn/about.html`, `en/about.html`
- Logos and icons: `assets/images/`
- Colors and component styling: `assets/css/nav.css` and the Xenon CSS files in `assets/css/`
- Default language redirect: `index.html`

The original advertising and analytics IDs have been removed. Add your own analytics only after you choose a provider and create your own site ID.
