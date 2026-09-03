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
- Chosen structure: browser archive with a sticky index, assigned structure 6,
  seed `72cd799b`.
- Approved comp: `.impeccable/mocks/gallery/01-sticky-archive.png`.

The first viewport pairs a compact archive index with one dominant browser
stage. Switchyard Cycle and Seeded Identity are live sandboxed local previews;
Absurdly Rational and 7Gradi use their existing screenshots at natural ratio
with full-resolution links. The gallery never calls a screenshot a full page,
never invents a project URL, and keeps status and stage context beside every
artifact.

Implementation inventory: semantic header/index/stages in HTML; archive layout,
browser bars, active-rule motion, and responsive stacking in CSS; active index
state in IntersectionObserver. The gallery directly displays only the existing
project rasters; its Switchyard iframe loads that sample's separate generated,
text-free background. Ground `#fbfaf9`, ink `#10111f`, rule `#dedee4`, accents
`#6b41fc`, `#4a7cff`, `#22bfc6`, and `#ffd84d`. No new gallery screenshot or
raster is required.
