# Lumina: The Cloud Garden — website

The marketing site for **Lumina: The Cloud Garden**, the gentle sky-garden game from
[Brewster Wickersham Publications](https://www.brewsterwickershampublications.com/). Plain static
HTML and CSS, made for GitHub Pages. No build step.

| File | What it is |
| --- | --- |
| `index.html` | The home page |
| `support.html` | Support and common questions |
| `privacy.html` | Privacy policy (same text as the app repo's `docs/privacy.html`; `#delete` anchor kept) |
| `site.css` | Shared styles |
| `images/` | The banner and six store screenshots, resized from the app repo's `docs/press/` |

Preview locally with `python -m http.server` in this folder and open http://localhost:8000.

## Status

Live at https://www.luminacloudgarden.com/ (GitHub Pages, custom domain, DNS at Porkbun). Canonical, Open Graph and
JSON-LD tags are set. The Google Play button is live (`com.wickersham.lumina`).

## Still to do

1. **App Store button** — when the iOS listing is live, replace the `store-btn soon` span in
   `index.html` with a link (the comment above it has the markup), and add the App Store URL to
   the JSON-LD.
2. **Search Console** — verify the domain by DNS TXT and submit the home page.
3. **Publisher site** — make sure brewsterwickershampublications.com links here.

The store listings currently use the policy pages at
`https://pennwickersham.github.io/Lumina-The-Cloud-Garden/`. If you switch them to the new domain,
keep the privacy text identical in both places until the old URLs are retired.
