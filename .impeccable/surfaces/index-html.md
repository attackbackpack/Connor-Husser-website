---
version: 1
slug: index-html
primary_target: index.html
related_targets:
  - websites/index.html
---

# Root portfolio surface

- Mode: Experience.
- Audience: college reviewers, collaborators, and general visitors.
- Job: explore Connor’s thinking through five artifact-led, truthful records.
- Primary action: View my work. Secondary: Business websites at `/websites/`.

The first viewport uses the simpler “Useful things, thoughtfully made.” headline
and a concise first-person explanation beside a real Absurdly Rational screenshot
labeled “Published website.” Project records alternate across the full page
rather than becoming a card grid, and each uses native details for Problem, Role,
Decisions, and Built while keeping Status adjacent.

Queen’s shows only a neutral synthetic flow, never real hospital geometry,
maps, handouts, or implied approval. The three local screenshots are the only
raster proof. Screenshot records preserve each image’s natural ratio instead
of cover-cropping it to the text column. The lower Seeded Identity canvas is a
slow decorative field, not project data. The route remains usable with no script,
reduced motion, forced colors, keyboard navigation, and a narrow phone viewport.
The surface inherits the published Seeded Identity UI: warm paper, deep ink,
thin rules, uppercase microtype, square controls, the original four-dot brand,
and violet, azure, mint, and yellow accents.

Shared navigation keeps a one-pixel ink underline on hover. The current item
uses an 8px internal gap and an adjacent 10px violet square; on the root,
Projects, About, and Contact update `aria-current="location"` immediately for
same-page clicks, the initial hash, and `hashchange`. An IntersectionObserver
tracks `#top`, `#projects`, `#about`, and `#contact`, clearing current at `#top`;
hash/click behavior remains the fallback.
