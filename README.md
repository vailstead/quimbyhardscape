# Quimby Hardscape & Construction

Static marketing site for **Quimby Hardscape & Construction**, a hardscape-focused landscaping business serving **Central and Southern New Hampshire**.

## Site contents

- `index.html` – single-page marketing site
- `assets/styles.css` – site styling
- `.github/workflows/deploy-pages.yml` – GitHub Pages deployment workflow
- `.nojekyll` – serves the site as plain static files

If the business uses a different inbox, update the `mailto:` links in `index.html`.

## GitHub Pages deployment

1. In GitHub, open **Settings → Pages**
2. Set **Source** to **GitHub Actions**
3. Merge this branch into your default branch
4. The workflow will publish the site automatically

## AWS DNS setup

If you want to use a custom domain managed in AWS Route 53:

1. Create the custom domain in your DNS zone
2. In GitHub Pages settings, add that custom domain
3. Add the DNS records that GitHub Pages provides for your domain
4. If you later decide on a final domain name, add a `CNAME` file to this repository containing only that hostname

For an apex domain, use the A/ALIAS records that GitHub Pages documents. For a subdomain such as `www`, use a CNAME record pointing to your GitHub Pages host.
