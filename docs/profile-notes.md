# Profile design and maintenance

## Intent

The public GitHub profile of **Cynrath** showcases independent software engineering, production web systems, automation and developer tooling. Lead with proof through real public repositories, not claims or vanity counters.

## Assets

- `assets/banner.svg` — 1200 × 390 editorial identity header, subtle native SMIL motion on technical orbit only.
- `assets/agent-context-kit.svg` — 560 × 245 project illustration.
- `assets/ackit-spec-kit-bridge.svg` — 560 × 245 project illustration.
- All images are committed locally, with no remote fonts, CDN images, JavaScript, or external stats widgets.
- Text and core visuals remain legible if SVG animations are blocked.
- GitHub may proxy/sanitize SVG images; browser-specific playback must be checked on rendered profile (not only raw source).
- Design uses a fixed dark surface so it is consistent on GitHub's light and dark site themes.

## Privacy

Never publish personal/legal names, phone numbers, personal e-mail, client names, customer systems, unpublished work, credentials, private URLs or repositories. Keep the public handle `Cynrath` consistent.

## Content

- Keep featured work tied to the actual public repositories and remove broken links promptly.
- Avoid fake metrics, dynamically generated GitHub activity cards, unsupported personal claims, busy badge walls, and gratuitous emojis.
- Prefer short, accurate summaries. The README must remain readable on both mobile and desktop.
- Keep brand copy in English on public-facing profile; internal notes may be Turkish or English.

## Release verification

1. Parse all SVGs as XML, verify safe self-contained markup, and rasterize them to ensure text stays within bounds.
2. Preview GitHub-flavored HTML layout at desktop and mobile widths.
3. Verify every relative image path exists and links point to the correct repositories.
4. Inspect the actual profile after merging; confirm if animated motion renders under GitHub's image proxy.
5. Only merge after visual review. Do not change unrelated repositories or profile account settings in this change.
