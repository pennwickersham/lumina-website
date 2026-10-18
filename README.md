# Lumina: The Cloud Garden — website

The marketing site for **Lumina: The Cloud Garden**, the gentle sky-garden game from
[Brewster Wickersham Publications](https://brewsterwickershampublications.com/). Plain static
HTML and CSS, made for GitHub Pages. No build step.

| File | What it is |
| --- | --- |
| `index.html` | The home page |
| `support.html` | Support and common questions |
| `privacy.html` | Privacy policy (same text as the app repo's `docs/privacy.html`; `#delete` anchor kept) |
| `404.html` | Not-found page (GitHub Pages serves it for any missing URL; root-relative paths, `noindex`) |
| `site.css` | Shared styles, including the shared "From Brewster Wickersham Publications" footer block |
| `robots.txt`, `sitemap.xml` | Crawler rules and the sitemap. Update `<lastmod>` when a page's content changes |
| `favicon.ico`, `favicon.png`, `apple-touch-icon.png` | Site icons |
| `images/` | The banner and six store screenshots, resized from the app repo's `docs/press/` |

Preview locally with `python -m http.server` in this folder and open http://localhost:8000.

## Status

Live at https://www.luminacloudgarden.com/ (GitHub Pages, custom domain, DNS at Porkbun). Every indexable page has a canonical URL, Open Graph and Twitter tags,
and the home page has `VideoGame` + `MobileApplication` JSON-LD. Every page's footer links to the other
Brewster Wickersham Publications sites and to the Amazon author store and book listings. The Google Play button is live (`com.wickersham.lumina`).

## Still to do

1. **App Store button** — when the iOS listing is live, replace the `store-btn soon` span in
   `index.html` with a link (the comment above it has the markup), update the "Is Lumina on iPhone
   and iPad?" FAQ answer, and in the JSON-LD add `iOS` to `operatingSystem`/`gamePlatform` and the
   App Store URL to `sameAs`.
2. **Search Console** — verify the domain by DNS TXT and submit `https://www.luminacloudgarden.com/sitemap.xml`.
3. **Publisher site** — make sure brewsterwickershampublications.com links here.

The store listings currently use the policy pages at
`https://pennwickersham.github.io/Lumina-The-Cloud-Garden/`. If you switch them to the new domain,
keep the privacy text identical in both places until the old URLs are retired.
