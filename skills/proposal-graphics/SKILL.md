---
name: proposal-graphics
description: >-
  Turn proposal messages into compliant, persuasive visuals — action captions written first, then
  feature/benefit tables, ghosting comparison graphics, process/swimlane diagrams, callout boxes,
  org charts, and past-performance cards — styled with PSS brand tokens and built accessibly. Use
  whenever anyone needs a proposal graphic, action caption, feature/benefit table, comparison table,
  process diagram, callout/pull-quote, org chart, cover graphic, or "make this section visual." Bridges
  the APMP graphics doctrine and the brand tokens into rendered output. Pairs with the Proposal Builder
  and brand skills; run the 508 pass on the final document.
---

# GovCon Proposal Graphics

Produces the visuals that raise win rates (visual-aided content is ~43% more persuasive and improves
recall). This is the *production* skill; the **APMP** skill owns the doctrine and **paradigm-brand-
guidelines** owns the look. Always finish with the **508** pass.

## The non-negotiable process (from APMP)

Every graphic follows this order — never render first:

1. **Action caption first.** Write the one-sentence message the graphic must land (a benefit, not a
   label): "Our phased transition keeps USACE operations running with zero downtime," not "Transition
   Plan." The caption is the point; the visual supports it.
2. **Summarize** the message in one sentence → **Explain** with the supporting detail → **Visualize**
   the concept → **Render** to a compliant, on-brand graphic.
3. **Validate** — Goal (answers a real evaluator question / shows why to pick PSS?), Content
   (understandable without the caption?), Aesthetics (every choice purposeful and consistent?). Have
   someone outside the team confirm it reads clearly.

Create key graphics **early** — the executive-summary graphic doubles as a proposal roadmap and a
storyboarding tool.

## Graphic types & when to use each

- **Feature → Benefit → Proof table** — the workhorse. Three columns: what we do / what it means for
  you / evidence. Forces the "So what?" test into the layout.
- **Ghosting comparison** — a tradeoff/approach table that raises the weakness of the alternative a
  competitor offers **without naming them** ("Approaches that rely on X risk Y; our approach…").
  Use independent/third-party evidence so it's defensible.
- **Process / phase / swimlane diagram** — transition plans, QC workflows, escalation paths. Show
  owners (swimlanes) and decision points; annotate each stage with its benefit.
- **Callout box / theme statement** — boxed, consistently formatted; carries a win theme or proof
  point. Format identically everywhere so evaluators learn to look for them.
- **Org chart / key-personnel map** — lines of authority, availability, and clearance at a glance;
  tie roles to labor categories.
- **Past-performance card** — one relevant contract per card, skimmable: agency, value, period,
  scope keywords (mirroring the SOW/PWS), CPARS rating, one-line result.
- **Metric / stat block** — a single quantified benefit made large and visual (payback period, %
  savings, on-time rate). One idea per block.

## Compliance & quality rules

- **Brand tokens** — pull colors/typography from `paradigm-brand-guidelines`; one primary accent per
  graphic; never pure black; consistent icon/style vocabulary. Confirm the `⚙ CONFIRM` tokens are set.
- **Accessibility (feeds 508)** — real alt text that conveys the *point* (not "chart"); contrast
  ≥ 4.5:1; never color-alone to convey meaning (add labels/patterns); real table structure with
  header rows, not a picture of a table where text is expected.
- **Copyright** — don't use images you don't have rights to; confirm commercial (not editorial-only)
  licensing; images are copyrighted by default.
- **Fit the page** — build at final display size; respect the RFP's page/format limits; graphics
  appear *after* they're referenced and carry the action caption.
- **No visual noise** — no textured backgrounds or decoration that doesn't carry meaning; simplify to
  the single message.

## Rendering notes (this environment)

- **In-document (Word/PDF proposals):** build feature/benefit and comparison content as **real tables**
  (accessible + editable), not flattened images. Diagrams as clean vector (SVG) placed inline.
- **Decks/one-pagers:** SVG or native shapes; keep to the brand palette so exports read as PSS.
- **Inline/interactive (CRM widgets):** the CRM can render SVG/HTML visuals; keep them on-brand and
  captioned.
- Prefer **vector** for diagrams/logos (crisp at any size); raster only for photos, licensed and at
  final resolution.

## Anti-patterns

- Rendering before the action caption exists (the #1 cause of wasted graphics).
- A "chart" that's really a decorative label with no message.
- Naming competitors in a ghosting graphic, or ghosting without independent evidence.
- Flattening a data table into an image (breaks accessibility and editing).
- Rainbow palettes, pure black, inconsistent callout formatting.
- Cramming multiple messages into one graphic — one caption, one point.
