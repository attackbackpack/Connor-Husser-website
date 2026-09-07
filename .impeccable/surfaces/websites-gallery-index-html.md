---
version: 1
slug: websites-gallery-index-html
primary_target: websites/gallery/index.html
related_targets:
  - websites/index.html
  - websites/samples/switchyard/index.html
  - index.html
---

# Website gallery surface

- Mode: Experience.
- Audience: local-business owners and reviewers who want to inspect the work.
- Job: see large, uncropped website previews and open live samples where they
  exist.
- Primary action: Explore the previews. Secondary: Open a live sample where
  available.

The first viewport opens with “Website gallery” and a compact archive index; the
active first stage is the real Absurdly Rational screenshot labeled “Published
website,” with an original full-resolution link. Seeded Identity and Switchyard
Cycle are live sandboxed local previews. 7Gradi displays the authorized WebP
derivative at its natural ratio and links to the original PNG. The gallery never
calls a screenshot a full page, never invents a project URL, and keeps status and
stage context beside every artifact.

Implementation inventory: semantic header/index/stages in HTML; browser-archive
frames with three dots, multicolor index marks and accent bars, active-rule
motion, and responsive stacking in CSS; active index state in
IntersectionObserver. The gallery uses existing project proof sources; its
Switchyard iframe loads that sample’s separate generated, text-free background.
The published-style system uses paper `#fbfaf9`, ink `#10111f`, body `#414251`,
muted `#696a79`, rule `#dedee4`, violet `#6b41fc`, azure `#4a7cff`, mint
`#22bfc6`, yellow `#ffd84d`, frame `#efedf5`, and 44px tap targets. No new
gallery screenshot or raster is required.

Shared navigation keeps a one-pixel ink underline on hover. A current item has
an 8px internal gap and an adjacent 10px violet square; Websites uses
`aria-current="location"` on this gallery route. The root’s Projects, About,
and Contact links update `aria-current="location"` immediately for same-page
clicks, the initial hash, and `hashchange`; an IntersectionObserver tracks
`#top`, `#projects`, `#about`, and `#contact`, clearing current at `#top`, with
hash/click behavior as the fallback.
