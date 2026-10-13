# Octavian — DevOps & SRE

A responsive, accessible personal services page. Static HTML and CSS, with no build step or JavaScript dependencies.

## Preview

Run `python3 -m http.server 8080` from this directory and open http://localhost:8080.

## Content

Edit `index.html` for services, contact links, and copy. Edit `style.css` for styling. The contact link currently points to the GitHub profile; replace it with a preferred email, booking link, or professional profile when ready.

The infrastructure diagram is illustrative. No client results, certifications, or performance guarantees are claimed. Google Fonts supplies optional fonts; system fallback fonts are included.

## Deployment

GitHub Pages can serve this directory directly. Configure Pages to deploy from the root of the `main` branch. The `.nojekyll` file disables Jekyll processing. All asset paths are relative, so the page supports both project URLs and custom domains.
