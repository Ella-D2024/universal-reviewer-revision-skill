---
name: universal-editable-ppt
description: Create or revise editable 16:9 academic, research, award-defense, interview, teaching, and professional presentation decks from source files, outlines, or reference screenshots, with strong visual hierarchy, native editable objects, and strict render-based alignment QA.
---

# Universal Editable PPT Skill

## 1. Purpose

Use this skill when the user asks to create, redesign, optimize, or revise a PowerPoint presentation, especially for:

- Academic presentations
- Scholarship or award defenses
- PhD/postdoc/job interviews
- Faculty teaching/research position interviews
- Research project reports
- Grant or talent-program defenses
- Thesis/doctoral milestone presentations
- Professional research summaries

The output should prioritize four goals:

1. **Clear content logic**
2. **Professional academic visual design**
3. **Native editability**
4. **Reliable layout without text-box misalignment, overflow, or overlap**

Do not include any user-specific identity, institution, research topic, or personal information unless it is explicitly supplied in the current task.

---

## 2. Default Output Standard

Unless the user specifies otherwise:

- Slide ratio: **16:9 widescreen**
- Background: light neutral academic background, not harsh pure white
- Main visual style: minimal, academic, professional, restrained
- Editable objects: titles, body text, tables, cards, shapes, timelines, arrows, labels, and charts must remain editable
- Use raster images only for photos, screenshots, illustrations, or decorative visuals that do not need editing
- Avoid decorative clutter, excessive gradients, heavy shadows, ornamental borders, cartoon icons, and stock-template effects
- Use consistent alignment, spacing, corner radius, stroke weight, font hierarchy, and page margins throughout the deck

Recommended default palette for academic decks:

- Background: warm light gray / light cream / light blue-gray
- Primary: deep red, burgundy, navy, or institutional accent
- Secondary: low-saturation tint of the primary color
- Text: near-black / charcoal
- Supporting lines: light gray or light tint of the primary color

If reference screenshots are provided, infer the palette, hierarchy, card treatment, header treatment, and spacing system from them rather than blindly applying this default.

---

## 3. Source Priority

When multiple sources exist, use this priority:

1. User-supplied content files and factual materials
2. User-supplied previous PPT
3. User-supplied reference screenshots/images
4. User-supplied outline or written instructions
5. General academic presentation conventions

Do not invent factual accomplishments, publication counts, awards, project names, dates, affiliations, rankings, or metrics.

If content is missing, use clearly marked editable placeholders such as:

- `[Name]`
- `[Institution]`
- `[Project Title]`
- `[Publication Count]`
- `[Insert Figure]`

---

# 4. Content Architecture Workflow

Before styling, first determine the presentation logic.

For personal academic/research presentations, prefer a concise narrative such as:

1. Profile / Background
2. Academic or career trajectory
3. Research experience
4. Research outputs
5. Projects / practical research experience
6. International or academic exchange
7. Research capabilities / methods
8. Honors or representative achievements
9. Future plan
10. Closing

For research-centered presentations, use:

1. Background / motivation
2. Core question
3. Research framework
4. Method
5. Results
6. Representative contributions
7. Validation
8. Discussion
9. Future work
10. Conclusion

For a short defense or interview, do not force every possible module into the deck. Keep only modules that directly help evaluation.

---

# 5. Slide Planning Rules

## 5.1 One Slide, One Message

Every slide should have one dominant message.

Avoid slides that simultaneously try to show:

- Biography
- Full publication list
- Multiple unrelated photos
- Project history
- Skills
- Awards

If necessary, split into two slides.

## 5.2 Use Evidence, Not Decorative Density

Prefer:

- 3 representative publications instead of 15 full citations
- 3 projects with roles/contributions instead of a paragraph
- 4 key metrics instead of a full CV table
- 2–5 representative photos instead of a photo wall with tiny images

## 5.3 Slide Count

Typical deck lengths:

- 5-minute defense: 8–12 slides
- 8–10-minute interview: 10–15 slides
- 15-minute academic presentation: 15–20 slides

Adjust to the actual speaking time when known.

---

# 6. Typography System

Use a clear, conservative academic font system.

## Default font sizes

- Cover title: 30–40 pt
- Section or slide title: 24–30 pt
- Card/module title: 19–23 pt
- Main body: **around 18 pt**
- Secondary notes: 15–17 pt
- Figure caption: 14–16 pt

Body text should generally be around **18 pt**, but it may be adjusted for legibility and information density.

Do not shrink body text excessively to force content into a box.

## Line spacing

Default body line spacing: **approximately 1.5**.

Allow adaptive adjustment between roughly 1.2 and 1.5 when:

- the text is very short
- a card has limited height
- Chinese text visually appears too loose at 1.5
- a title block requires compact spacing

Maintain comfortable spacing and avoid cramped text.

## Paragraph spacing

Use paragraph spacing instead of repeated manual line breaks.

Prefer:

- 4–8 pt after short bullet paragraphs
- 8–12 pt between conceptual blocks

---

# 7. Alignment and Text-Box Safety Rules

This section is mandatory. Text-box misalignment is a critical failure.

## 7.1 Use a Layout Grid

Define slide-safe margins first.

Recommended widescreen working margins:

- Left: 0.45–0.65 in
- Right: 0.45–0.65 in
- Top: 0.30–0.50 in
- Bottom: 0.30–0.50 in

All content should align to a consistent invisible grid.

## 7.2 Card Geometry

For each card/module:

1. Create the background/card shape first
2. Define internal padding
3. Create the text box inside the padded safe area
4. Keep the text box fully inside the card
5. Use matching X/Y coordinates across repeated cards

Recommended internal card padding:

- Horizontal: 0.18–0.30 in
- Vertical: 0.12–0.22 in

Do not position text visually by guessing.

## 7.3 Text Containment

For every text box:

- Text must remain inside its intended shape/card
- No baseline should touch the card border
- No line should extend outside the card
- No title should overlap decorative shapes
- Avoid automatic font shrinking unless absolutely necessary
- Prefer increasing box height or reducing text volume before reducing font size

## 7.4 Repeated Components

Cards in the same row must share:

- identical height
- consistent width or deliberate proportional width
- identical top alignment
- identical title baseline
- consistent inner padding

## 7.5 Centered Text

If text is meant to be vertically centered inside a pill/button/card, use actual vertical alignment settings rather than manually adjusting with spaces or extra line breaks.

## 7.6 Text and Shape Grouping

Whenever possible, group logically related objects after alignment:

- card + card title + card body
- timeline marker + year + description
- metric value + metric label

This reduces accidental movement during future editing.

---

# 8. Recommended Slide Layout Library

Use these layouts as modular patterns.

## A. Profile Layout

- Left: identity/photo block or visual identity block
- Right: education/background information
- Bottom: timeline or key metrics

If the user says **no personal photo**, do not reserve or show a portrait frame. Replace it with:

- typographic identity block
- abstract academic visual
- institutional motif
- key metrics

## B. Two Equal Columns

Use for:

- Two projects
- Two international experiences
- Two case studies
- Two figures

## C. Top Summary + Large Bottom Visual

Use for:

- Research framework
- Career trajectory
- Project architecture
- Main concept + large figure

## D. 2×2 Grid

Use for:

- Four competencies
- Four representative activities
- Four research outputs
- Four photos

## E. Five-Item 2+3 Layout

Use two items in the top row and three in the bottom row, centered as a balanced pyramid.

Use for:

- Honors
- Research outputs
- Conference and international experience photos
- Capability modules

## F. Three-Card Project Layout

Each project card should contain:

- Role
- Project title
- 2–4 concise contribution lines
- Optional one metric or representative visual

## G. Timeline

Use for education, career, research progression, or future plan.

Timeline should be visually simple. Avoid tiny explanatory paragraphs under each node.

---

# 9. Cover Slide Rules

The cover must feel intentionally designed rather than being a blank title on a background.

If the user provides an exact title, preserve it exactly.

Recommended cover structure:

- Strong primary title
- Short subtitle/tagline if appropriate
- Presenter / organization / date information
- One restrained visual device, such as:
  - gradient title band
  - geometric academic motif
  - structured timeline strip
  - four small thematic modules
  - subtle institutional pattern

Do not place a personal portrait on the cover unless explicitly requested.

Avoid large empty regions that feel accidental.

---

# 10. Color and Background Rules

Do not default to pure white if the user prefers a softer academic style.

Good background alternatives:

- #F7F5F2 warm ivory
- #F5F6F7 light neutral gray
- #F3F6F8 light blue-gray
- #FAF6F5 warm red-tinted neutral

For deep-red academic style, a useful structure is:

- Deep burgundy/red header
- Light red-tinted section background
- White or near-white cards
- Burgundy accent labels
- Soft gray separators

Keep contrast high enough for projection.

---

# 11. Reference-Image Adaptation

When reference screenshots are supplied:

Analyze and reproduce the **design language**, including:

- dominant color family
- title bar position
- logo position
- card shape
- section header style
- stroke thickness
- use of gradient or solid fills
- white-space density
- relative font hierarchy
- table style
- timeline style
- image arrangement

Do not simply screenshot and paste the reference slide as the new slide.

Reconstruct core elements as native editable PowerPoint objects.

Use generated images only when the reference contains non-editable illustration or decorative artwork that cannot reasonably be recreated with shapes.

---

# 12. Tables

Academic tables must be readable from a screen.

Rules:

- Avoid more than 6–7 columns unless absolutely necessary
- Use concise labels
- Emphasize key rows/metrics rather than showing all CV-level detail
- Use light separators instead of heavy full borders
- Keep header typography distinct
- Avoid tiny body font

When a publication table becomes dense, replace it with representative publication cards plus a summary metric.

---

# 13. Image and Visual Handling

Images should be cropped consistently.

Use:

- consistent aspect ratios within the same visual group
- aligned image tops/bottoms
- captions directly below the corresponding image
- identical caption widths for repeated images

Avoid:

- distorted images
- inconsistent corner radii
- random image sizes
- images touching slide edges

If image placeholders are needed, create clearly labeled editable placeholders such as `[Insert Conference Photo]`.

---

# 14. Editability Rules

Core content must remain editable.

Prefer native PowerPoint objects for:

- Text
- Cards
- Tables
- Timelines
- Arrows
- Process flows
- Simple diagrams
- Numerical metrics
- Labels

Do not flatten an entire slide into one image unless the user explicitly requests a non-editable visual deck.

If AI image generation is used, it should mainly support:

- decorative backgrounds
- non-critical illustrations
- abstract visuals

Critical facts and labels must remain native editable text.

---

# 15. Visual QA: Mandatory Render-and-Inspect Loop

Before delivering the final PPT, perform a render-based quality-control pass.

## Pass 1: Structural Check

For every slide, verify:

- slide title is present and aligned
- title does not overlap the header
- footer/page marker is consistent
- cards do not overlap
- images stay within frames
- no objects extend outside slide boundaries

## Pass 2: Text Check

For every text box, verify:

- text is inside the intended card
- no clipping
- no overflow
- no unexpected line wrap
- no single-character orphan line when avoidable
- title and body are visually centered where intended
- line spacing looks appropriate
- body font is generally around 18 pt

## Pass 3: Alignment Check

Visually inspect repeated objects:

- same row = same top alignment
- same column = same left alignment
- repeated cards = same internal padding
- metric cards = consistent number baseline
- captions = aligned with image widths

## Pass 4: Projection Check

Ask:

- Can the smallest text be read on a projector?
- Is there enough contrast?
- Is each slide understandable in 5–10 seconds?
- Is the slide too dense?

If the answer is no, simplify the slide.

## Pass 5: Final Montage Check

Render all slides and inspect them together as a montage/contact sheet.

This catches:

- inconsistent header positions
- sudden background changes
- font-size drift
- inconsistent visual density
- misaligned page numbers
- cards with different heights

Do not deliver the PPT before this check is completed.

---

# 16. Common Failure Modes and Corrections

## Failure: Text and card become misaligned

Correction:

- rebuild using shared X/Y coordinates
- set card first, then calculate text position from card bounds
- use fixed internal padding
- group after alignment
- render and visually inspect

## Failure: Body text too small

Correction:

- shorten text
- split the slide
- reduce number of modules
- enlarge the text box
- keep body around 18 pt whenever possible

## Failure: Slide is too white / visually flat

Correction:

- add a very light neutral background tint
- introduce a restrained title gradient/bar
- use subtle section bands or card fills
- maintain large white-space areas without making the slide visually empty

## Failure: Cover looks unfinished

Correction:

- create a designed title composition
- add a structured visual motif
- use a strong accent block or timeline strip
- keep the cover clean but intentional

## Failure: Too many publication citations

Correction:

- show 3–5 representative outputs
- highlight journal level / role / contribution
- move the full list to appendix if needed

## Failure: Reference style copied only superficially

Correction:

- reconstruct the reference system: header, spacing, cards, hierarchy, geometry, background, and typography
- do not merely change the color palette

---

# 17. Final Delivery Checklist

Before final delivery confirm:

- [ ] 16:9 ratio
- [ ] exact user-specified title preserved
- [ ] requested cover constraints followed
- [ ] all critical content editable
- [ ] body font around 18 pt unless justified otherwise
- [ ] line spacing approximately 1.5 with adaptive adjustment where needed
- [ ] no text outside boxes
- [ ] no overlapping objects
- [ ] no clipped text
- [ ] no accidental pure-white background when a tinted background was requested
- [ ] consistent header/footer system
- [ ] consistent card padding
- [ ] images proportionally cropped
- [ ] every slide rendered and checked
- [ ] montage inspected for cross-slide consistency
- [ ] output file opens correctly

---

# 18. Recommended Response Pattern

When the PPT is complete, respond concisely with:

1. What was created or revised
2. Important design constraints implemented
3. A direct download link to the editable `.pptx`

Do not claim that alignment or rendering was checked unless it was actually rendered and inspected.
