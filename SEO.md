# Search discovery and maintenance

The public site is https://octavianandrei.github.io/.

## What is implemented

- Descriptive page titles and summaries; canonical URLs for the homepage and six service pages.
- Server-delivered HTML with all service text and navigable links, without a JavaScript rendering requirement.
- JSON-LD describing the provider as a Person, the WebSite, service WebPages, Services, and breadcrumbs. This does not imply eligibility for a specific Google rich result.
- `/robots.txt` allows all crawlers, including search and AI crawlers, and points to `/sitemap.xml`.
- An XML sitemap with canonical page URLs and the actual last significant update date.
- `/llms.txt` as an optional summary for tools that choose to consume it. It is not a ranking signal or substitute for HTML, a sitemap, or webmaster registration.
- LinkedIn and WhatsApp contact links supplied by the site owner.
- A public IndexNow ownership key file. This is a public URL-verification token by design, not a private API credential.

## Google Search Console: account step

1. Sign in at https://search.google.com/search-console/.
2. Add a **URL prefix** property: `https://octavianandrei.github.io/`. GitHub controls the github.io domain, so use the URL prefix rather than DNS verification for that domain.
3. Choose **HTML file** verification. Download the exact file Google provides and add it to the repository root without changing its contents. Alternatively, use the HTML meta tag Google provides in `index.html`.
4. Wait for GitHub Pages to deploy, then click **Verify**. Keep the verification file or tag in the repository afterward.
5. Submit `https://octavianandrei.github.io/sitemap.xml` in **Sitemaps**.
6. Inspect the homepage URL and request indexing. Review indexing and search performance as data becomes available.

## Bing Webmaster Tools: account step

Sign in at https://www.bing.com/webmasters/ and add the same site. Import the verified Search Console property if offered, or use the exact XML file or meta tag Bing provides. Submit the sitemap. IndexNow notifications do not create or verify a Webmaster Tools account property.

## Future updates

Update sitemap `<lastmod>` dates only when a page's content or structured data materially changes. Add new canonical pages to the sitemap and link to them from existing relevant pages. Submit changed URLs through https://www.indexnow.org/documentation after the content and ownership key file are live. Do not repeatedly submit unchanged URLs.

Crawl permission and URL submission do not guarantee indexing, placement, rich results, or AI citations. Useful original evidence such as genuine project writeups and public technical work can strengthen the service descriptions; do not add invented customers, reviews, credentials, or results.
