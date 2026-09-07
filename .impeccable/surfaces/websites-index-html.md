---
version: 1
slug: websites-index-html
primary_target: websites/index.html
related_targets:
  - index.html
---

# Websites service surface

- Mode: Persuade.
- Audience: local-business owners.
- Job: understand Connor’s personal accountability and the sequence Presence
  Check → Website Build → Owner Handoff.
- Primary action: View website work. Secondary: See how I work.
- Visible work route: a website-only index leading to the dedicated gallery,
  not a client-results claim.

The visual skin follows the published Seeded Identity system: warm paper
(`#fbfaf9`), deep ink (`#10111f`), muted body text, thin rules, Barlow and
Barlow Condensed, the original four-dot mark, square ink buttons with yellow
hover, pale-violet proof frames (`#efedf5`), and violet/azure/mint accents.
The identity field remains lower on the page, and its decorative controls keep
their current behavior and accessibility treatment.

The hero uses “A better website for the business you built.” with short
first-person copy about reviewing, building, and handing the working pieces back
to the owner. It leads with a real Absurdly Rational screenshot labeled
“Published website.” Its Clarity, Proof, and Connection ranges are explicitly
decorative, show live values, update the slow canvas, and Reset field restores
64/58/52. The work index names Absurdly Rational, Seeded Identity, Switchyard
Cycle, and 7Gradi Gelato; Rootwork stays on the personal portfolio as a study
tool rather than website-service proof. The 7Gradi concept is stated once as
unsolicited and never client work. Contact details are unresolved, so no
placeholder contact or form appears.

Shared navigation keeps a one-pixel ink underline on hover. A current item has
an 8px internal gap and an adjacent 10px violet square; Websites remains
`aria-current="page"` on this service route. The root’s Projects, About, and
Contact links update `aria-current="location"` immediately for same-page
clicks, the initial hash, and `hashchange`; an IntersectionObserver tracks
`#top`, `#projects`, `#about`, and `#contact`, clearing current at `#top`, with
hash/click behavior as the fallback.
