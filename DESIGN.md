---
name: Seeded Identity
description: A personal portfolio and local-business website service presented as an open exhibition table in the published Seeded Identity visual language.
colors:
  paper: "#fbfaf9"
  ink: "#10111f"
  body: "#414251"
  muted: "#696a79"
  rule: "#dedee4"
  frame: "#efedf5"
  violet: "#6b41fc"
  azure: "#4a7cff"
  mint: "#22bfc6"
  yellow: "#ffd84d"
typography:
  display:
    fontFamily: "Barlow, system-ui, sans-serif"
    fontSize: "clamp(3.5rem, 6.5vw, 6.5rem)"
    fontWeight: 500
    lineHeight: "0.9"
    letterSpacing: "-0.035em"
  editorial:
    fontFamily: "Barlow Condensed, Barlow, sans-serif"
    fontSize: "clamp(3rem, 6vw, 5.5rem)"
    fontWeight: 600
    lineHeight: "0.84"
    letterSpacing: "-0.03em"
  body:
    fontFamily: "Barlow, system-ui, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: "1.55"
rounded:
  none: "0"
spacing:
  gutter: "clamp(18px, 4.4vw, 64px)"
  tap: "44px"
components:
  button:
    height: "56px"
    border: "1px solid var(--ink)"
    textTransform: uppercase
  inlineAction:
    height: "44px"
    border: "1px solid var(--ink)"
    textTransform: uppercase
  disclosure:
    marker: native
    height: "44px"
---

# Design System: Seeded Identity

## Overview

**Creative North Star: “The open exhibition table.”**

The current local redesign supplies the structure: a proof-first portfolio, a
personal website-service route, a compact gallery, and a complete recovery page.
The published connorhusser.com interface supplies the visual language: warm
paper, deep ink, thin rules, uppercase microtype, the four-dot identity mark,
and four small seeded accents. The work, status, and decision record remain
more important than the surface styling.

The root portfolio is an Experience surface. The website route is Persuade.
The gallery is an Experience surface. All four pages share the same identity,
but the content order and behavior of each route remain distinct.

## Colors

- **Paper:** `#fbfaf9`, the shared page ground.
- **Ink:** `#10111f`, headings, borders, primary controls, and the safe flow.
- **Body:** `#414251`, long-form reading copy.
- **Muted:** `#696a79`, supporting labels and secondary metadata.
- **Rule:** `#dedee4`, one-pixel dividers.
- **Frame:** `#efedf5`, pale-violet proof and identity surfaces.
- **Violet / Azure / Mint / Yellow:** `#6b41fc`, `#4a7cff`, `#22bfc6`, and
  `#ffd84d`; used as the seeded identity accents, process markers, gallery
  index states, and decorative canvas line palette.

Selection is yellow with ink text. Focus is a visible `2px` ink outline with a
`4px` offset. No shadows, gradients, glass, or decorative blur are part of the
system.

## Typography

Barlow is self-hosted and handles body copy, general large headings, project
names, controls, and status text. General large headings use weight 500 with
tracking no tighter than `-0.04em`. Barlow Condensed 600 is reserved for
editorial section headings. Labels, navigation, preview bars, statuses, and
actions use uppercase Barlow 600 with deliberate letter spacing.

## Structure and composition

The root keeps the new proof-first order: a concise thesis beside the real
Absurdly Rational screenshot, then alternating artifact-and-record rows for
Absurdly Rational, Rootwork, Queen’s visitor wayfinding, 7Gradi Gelato, and
Seeded Identity, followed by About and Contact. The service route keeps its
direct hero proof, three-step process, honest website-work index, personal
accountability statement, lower identity field, and pending Contact state. The
gallery keeps Absurdly Rational first, then its compact index and large natural-
ratio previews. The 404 page keeps its complete heading and two recovery routes.

Proof frames use an ink border, pale-violet frame background, and an uppercase
preview bar. Images retain natural ratios. Live previews remain sandboxed.
The root’s project details remain native `<details>` elements with native
disclosure markers, 44px summaries, thin-rule separators, and the existing
Problem / Role / Decisions / Built facts. Statuses remain adjacent to their
records and are never replaced by decorative badges.

## Components

### Brand and navigation

The original brand is text in uppercase microtype with a 40×10px `::before`
mark containing four 8px dots in violet, azure, mint, and yellow. The favicon
is the original three-dot violet, azure, and mint mark. Navigation is uppercase
at `.78rem` with `.12em` tracking and 44px targets; hover keeps a one-pixel ink
underline. A current route uses `aria-current`, an 8px internal gap, and an
adjacent 10px square marker in violet. Websites is `page` on `/websites/`,
`location` on `/websites/gallery/`, and the 404 page has no current item. On the
root, the Projects, About, and Contact links update `aria-current="location"`
immediately on same-page clicks, the initial hash, and `hashchange`; an
IntersectionObserver tracks `#top`, `#projects`, `#about`, and `#contact`,
clearing current in `#top` and setting the matching section elsewhere, with
hash/click behavior preserved as the fallback.

### Buttons and actions

Buttons are square, 56px high, ink-bordered, uppercase, and `.8rem` with
`.1em` tracking. Primary buttons use ink with paper text; hover uses yellow
with ink text. Inline actions are 44px targets with an ink underline and turn
violet on hover.

### Decorative identity field

The root and service field are decorative only. Their existing deterministic
canvas code remains intact: it uses the violet/azure/mint/yellow palette,
requestAnimationFrame only while visible, pauses when the document or field is
offscreen, becomes static under reduced motion, and hides the canvas in
no-script and forced-colors modes. The service sliders remain decorative, keep
their live values and reset behavior, and use violet, azure, and mint accents.

## Accessibility and truth boundaries

- Keep skip links, semantic headings, keyboard-visible focus, native details,
  reduced motion, forced colors, no-script fallbacks, and the gallery’s numeric
  fragment observer fix.
- Keep project statuses explicit: published, personal/working, synthetic or
  fictional, and unsolicited/unapproved.
- Do not imply Queen’s approval, installed hospital guidance, client outcomes,
  or commercial results. Keep Contact pending until real details exist.
- Keep the optimized 7Gradi WebP as a display derivative of the authorized PNG;
  full-resolution links continue to point to the PNG.

## Do / don’t

### Do

- Let the artifact and status lead before explanation.
- Keep square geometry, thin rules, natural image ratios, and the published
  palette consistent across routes.
- Preserve the existing animation, responsive behavior, and safe fallbacks.

### Don’t

- Do not restore the old page wholesale; that would discard the new structure.
- Do not use generic card grids, pointless section numbers, overline kickers,
  gradient text, shadows, glass, or custom plus/minus disclosure glyphs.
- Do not invent contact details, claims, approvals, or project outcomes.
