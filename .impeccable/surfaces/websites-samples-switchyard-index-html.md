---
version: 1
slug: websites-samples-switchyard-index-html
primary_target: websites/samples/switchyard/index.html
related_targets:
  - websites/gallery/index.html
  - websites/index.html
---

# Switchyard Cycle fictional sample

- Mode: Persuade.
- Audience: a local cyclist who knows the symptom but not the repair term.
- Job: choose the closest symptom, see one honest starting point, and understand
  what an in-person diagnosis would do next.
- Chosen direction: velodrome lap board, grounded direction 7, seed `22ec0c2d`.
- Approved comp: `.impeccable/mocks/switchyard/01-service-board.png`.

The opening places the question in a track-blue field and a fixed three-slot
service board beside it. Selecting a slot changes only its yellow active state,
the screen-reader service label, and the explanatory copy. The sample explicitly
says that it is a fictional demonstration and never claims to diagnose a bicycle
online.

Implementation inventory: header, headline, CTA, service copy, service-depth
rows, process, symptom labels, and controls are semantic HTML. The hero ships
one generated, text-free raster at
`assets/projects/switchyard-workshop-board.png`; it supplies only the tactile
painted-track, diagonal lane seam, brushed-steel board, blank enamel plates,
arrows, fasteners, and mechanical counter. The approved comp was its reference,
not a shipping substitute. Exact raster origin and generation prompt are both
embedded in the PNG; the prompt is also preserved at
`.impeccable/assets/switchyard-workshop-board.prompt.txt`, and the complete
origin record is repeated in the adjacent `.origin.txt`. CSS positions
the semantic overlays and supplies active/focus states; minimal JavaScript keeps
the pressed state and screen-reader recommendation current. Palette: asphalt
`#07090b`, panel `#15191d`, track blue `#0b55a5`, deep blue `#06366e`, workshop
yellow `#ffd119`, chalk `#f7f4eb`, lane red `#d63f2f`, rule `#545a60`.
