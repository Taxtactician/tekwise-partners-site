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
