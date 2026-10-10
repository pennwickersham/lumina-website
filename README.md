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

## Launch checklist

1. **Buy the domain** (e.g. at Porkbun, like the other sites).
2. **Store buttons** — in `index.html`, replace the two `<span class="store-btn soon">` elements
   with real links (the comment above them has the markup and the Play URL,
   `com.wickersham.lumina`).
3. **Canonical and social tags** — uncomment / fill in the `LAUNCH` block in the `<head>` of
   `index.html`, and add `"url"` to the JSON-LD.
4. **Publish** — make the repository public, then Settings → Pages → Deploy from branch `main`,
   folder `/ (root)`.
5. **Custom domain** — add a `CNAME` file containing the domain (e.g. `www.example.com`), set it in
   Settings → Pages, point DNS at GitHub Pages (`A` records 185.199.108–111.153 for the apex, a
   `CNAME` to `pennwickersham.github.io` for `www`), then tick **Enforce HTTPS**.
6. **Search Console** — verify the domain by DNS TXT and submit the home page.
7. **Publisher site** — on brewsterwickershampublications.com, change Lumina's badge from
   "Coming soon" and add store buttons and a button for the new domain.

The store listings currently use the policy pages at
`https://pennwickersham.github.io/Lumina-The-Cloud-Garden/`. If you switch them to the new domain,
keep the privacy text identical in both places until the old URLs are retired.
