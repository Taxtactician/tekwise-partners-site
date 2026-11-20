# Tekwise Partners website

Static site for Tekwise Partners LLC, hosted on GitHub Pages.

## Pages
- `index.html` — home page (services, workshops teaser, affiliates, contact)
- `estate-planning.html` — estate planning workshops and the Estate Planning Checkup
- `css/style.css` — all styling; brand colors are the variables at the top

## Publishing on GitHub Pages
1. Push this folder to a GitHub repository.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, then **Save**.
4. The site appears at `https://<account>.github.io/<repo>/` within a minute or two.

## Custom domain (optional)
In **Settings → Pages → Custom domain**, enter the domain (for example `tekwisepartners.com`). GitHub adds a `CNAME` file. Then, at your domain registrar, add:
- For the root domain: four `A` records pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- For `www`: a `CNAME` record pointing to `<account>.github.io`

Turn on **Enforce HTTPS** once the certificate is issued.

## Editing
- Change colors in the `:root` block at the top of `css/style.css`.
- The header and footer are repeated in each page; update both files when changing them.

## SEO files
- `robots.txt`, `sitemap.xml` — for search engines (submit the sitemap in Google Search Console)
- `llms.txt` — plain-language summary of the business for AI assistants and AI search
- `img/og-image.png` — the preview image shown when the site is shared on social media or by text
- Each page has a title, meta description, canonical URL, social preview tags and schema.org structured data (JSON-LD)

All of these use `https://tekwisepartners.com`. If the site lives at a different address, find and replace that domain across the repo, and update `lastmod` dates in `sitemap.xml` when pages change.
