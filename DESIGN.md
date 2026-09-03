# Design system — Seeded Identity

## Shared rules

Seeded Identity is Connor Husser’s shared visual system: off-white paper,
deep ink, thin rules, mostly square geometry, and self-hosted Barlow plus
Barlow Condensed. Violet, azure, mint, and yellow live in a deterministic
canvas field seeded `eb2fb559`. The field is decorative only; it never carries
instructions, route data, contact details, or status.

Avoid generic cards, shadows, glass, gradient text, stock-agency presentation,
device mockups, and invented proof. Artifacts lead when they exist.

## Route modes and IA

| Route | Mode | Visitor | Primary task |
| --- | --- | --- | --- |
| `/` | Experience | College reviewers, collaborators, general visitors | Inspect five truthful project records. |
| `/websites/` | Persuade | Local-business owners | Understand Presence Check → Website Build → Owner Handoff. |
| `/websites/gallery/` | Experience | Local-business owners and reviewers | Inspect large, uncropped website previews and open live samples. |

Shared nav is Projects, Websites, About, Contact. Root links Projects,
About, and Contact in-page; the service route returns to root for Projects and
About, remains current for Websites, and has in-page Contact. A client footer
points to `/websites/`; a college application points to root.

## Root: Experience

The first viewport holds the exact thesis, “I design websites, tools, and
systems that make complicated things clearer.” It pairs a broad personal
perspective with a live Seeded Identity canvas. The primary action is Explore
my projects; Need a business website? is secondary. There are no sliders on
the root.

Five full-width alternating editorial records carry the artifact beside a
factual narrative. Every record visibly labels Problem, Role, Decisions,
Built, and Status. Queen’s uses only a neutral HTML/CSS flow: Known checkpoint
→ Approved destination → Route steps → Stop and ask staff if uncertain.
Raster artifacts keep their natural aspect ratio; their record copy may never
force them into a taller cover-cropped box.

## Websites: Persuade

The service route retains the Transformation Field as a live hero artifact and
its performance behavior: capped device pixels, `requestAnimationFrame`,
resize observation, visibility pause, and static reduced-motion render. The
three native controls are explicitly exploratory/decorative, retain visible
values, update field state/render, and the keyboard-accessible Reset field
action restores 64 / 58 / 52. Work uses only the three verified screenshots.
The Hawaii concepts are labeled once as unsolicited concepts, never client
work. The service work index contains only websites: Switchyard Cycle, Seeded
Identity, Absurdly Rational, and 7Gradi Gelato. No placeholders or rejection
narrative is rendered.

## Website gallery

The gallery is a browser archive, not a thumbnail grid. A compact sticky index
supports four oversized stages. Live local pages use sandboxed previews and
the two screenshot-only records use their full natural ratio with a direct
full-resolution link. Status and stage context stay adjacent to every artifact.

Switchyard Cycle is a separate fictional sample world documented inside its
own folder. Its workshop-yellow, track-blue, asphalt, and chalk system does not
replace Seeded Identity outside the sample frame.

## Accessibility, responsive, and links

- The skip link is first, focus is visible, headings and landmarks are
  semantic, and controls meet 44px minimum targets (primary links are 56px).
- Canvas is hidden under forced colors; reduced motion is static; no-script
  hides inert canvases/controls but keeps all essential content and status.
- Desktop records alternate in two editorial columns; phones stack in reading
  order. Gutters use `clamp(18px, 4.4vw, 64px)` and no layout may overflow
  horizontally.
- Link only verified routes and fragments. Do not publish a placeholder email,
  phone, mailto, fake CTA, unresolved project link, metric, approval, or claim.
- Production contact sections state that details are being finalized. Status
  text, not color, communicates project state.
