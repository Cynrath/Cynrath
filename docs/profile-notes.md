# GitHub profile — maintenance notes

## Scope

This is the public profile repository for [Cynrath](https://github.com/Cynrath). GitHub renders the root `README.md` on the user profile. The profile presents engineering work and publicly available repositories rather than a label describing which tools are used.

## Privacy

Do not add personal/legal names, direct contact details, credentials, private repository details, or client information to public profile content. Use **Cynrath**, matching the GitHub account and banner.

## Visual assets

- `assets/banner.svg` is a self-contained 1000 × 300 SVG.
- The banner uses native SVG shapes and declarative SMIL animation; it contains no JavaScript, external fonts, network requests, or remotely hosted graphics.
- The initial/static frame is complete and legible when animation is unavailable.
- Motion is deliberately limited to a slow signal along the workflow and a small status indicator.
- GitHub's standalone SVG preview may not animate. Check the rendered README on the actual profile in addition to inspecting the file.
- The banner is designed to stay legible against GitHub's light and dark page themes.

## Content rules

- Lead with software engineering, production web applications, infrastructure, and developer tooling.
- Keep technical claims grounded in published work.
- Avoid unnecessary badges, GitHub stat generators, rotating widgets, and third-party image services.
- Update project links and summaries when repositories change.
- Keep the README concise enough to scan on mobile.

## Review checklist

1. Check the banner SVG is valid XML and renders as a static image.
2. Inspect text clipping and legibility at desktop and narrow widths.
3. Review README links and image paths.
4. Verify the rendered [GitHub profile](https://github.com/Cynrath) after merging.
5. Check any motion in a real browser; if GitHub blocks it, retain the legible static banner.
