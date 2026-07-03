# Aadi Projects — Website

Static website for **Aadi Projects** (Consulting · Capital · Cofoundry), ready to deploy on **Cloudflare Pages** via GitHub.

## What's inside
- **67 pages** as clean directory URLs (each is `path/index.html`, served without `.html`).
- **Auto-hide header** (logo + menu) that slides away on scroll-down and returns on scroll-up; responsive mobile menu.
- **Baked footer** on every page (socials, Terms, Privacy, offices).
- **SEO on every page**: title, meta description, canonical, Open Graph, Twitter cards, and JSON-LD (Organization, WebPage, BreadcrumbList).
- **AI-search ready**: `robots.txt` (allows GPTBot, ClaudeBot, PerplexityBot, Google-Extended, etc.), `llms.txt`, `sitemap.xml`, structured data, semantic `<main>`.
- Assets: `assets/og.png` (social preview), `assets/favicon.svg`, `assets/icon-180.png`.
- Cloudflare config: `_headers`, `_redirects`, `404.html`.

## Deploy on Cloudflare Pages
1. Create a new **GitHub repository** and upload the entire contents of this folder (keep the structure).
2. In the **Cloudflare dashboard** → **Workers & Pages** → **Create** → **Pages** → **Connect to Git**, pick the repo.
3. Build settings:
   - **Framework preset:** None
   - **Build command:** *(leave empty)*
   - **Build output directory:** `/` (root)
4. Deploy. You'll get a `*.pages.dev` URL immediately.
5. Add your custom domain **www.aadiprojects.com** (and the apex) under **Custom domains**. Cloudflare handles SSL.

No build step is required — this is a plain static site.

## After deploy — do these
- Replace footer placeholders: office addresses, effective dates on `/privacy` and `/terms`, and the grievance-officer line.
- Confirm `www.aadiprojects.com` is the canonical host (the SEO tags assume it). If you use the apex, update canonicals/sitemap accordingly.
- (Optional) Submit `sitemap.xml` in Google Search Console and Bing Webmaster Tools.

## Editing
Every page is a standalone `.html` file with inline styles — open the folder's `index.html`, edit, commit, and Cloudflare redeploys automatically.
