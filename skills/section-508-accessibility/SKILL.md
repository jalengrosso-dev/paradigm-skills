---
name: section-508-accessibility
description: >-
  Make electronic deliverables and proposal documents conformant with Section 508 / WCAG AA — accessible
  PDFs and Word files, tagging and reading order, alt text, heading structure, table markup, color
  contrast, and link text — and produce or review a VPAT/ACR when a solicitation requires one. Use
  whenever anyone mentions Section 508, accessibility, WCAG, accessible PDF/Word, screen-reader
  compatibility, tagged PDF, alt text, color contrast, VPAT, ACR, or "does this deliverable meet
  federal accessibility requirements." Owns the accessibility conformance pass that no other agent
  covers; pair it as a final check on any federal-facing document or electronic deliverable.
---

# GovCon Section 508 Accessibility

Owns accessibility conformance for federal-facing electronic content. Runs as a **final pass** on
documents the CRM produces (proposals, capability statements, one-pagers, reports) and on any
electronic deliverable a contract requires. No other agent owns this.

## When 508 applies (and when it bites)

Section 508 requires federal agencies to make their **electronic and information technology (ICT)**
accessible to people with disabilities — and that obligation flows to contractors through
solicitation requirements. It shows up two ways:

1. **Deliverables under the contract** — software, websites, documents, training, or media delivered
   to or hosted by the agency must conform. This is where non-conformance becomes a **performance
   issue** (rejected deliverables, CPARS impact).
2. **Your proposal/submission itself** — some agencies require submitted PDFs to be accessible, and
   many evaluate accessibility approach for ICT work. Read **Section L/M and the SOW/PWS** for
   accessibility language; if it's there, treat it as a compliance requirement, not a nicety.

**The standard:** the Revised 508 Standards incorporate **WCAG Level AA** (2.0 as the formal baseline;
many agencies now expect **2.1 AA** — confirm which the solicitation cites). Conform to AA.

## Accessible document checklist (PDF & Word)

Apply to every federal-facing document. Most of these are set in the source (Word) and preserved on
export to tagged PDF.

- **Real heading structure** — use actual Heading 1/2/3 styles (not just bold big text); one logical
  outline, no skipped levels. Screen readers navigate by headings.
- **Reading order & tags** — export to **tagged PDF** with a correct reading order that matches the
  visual order; verify the tag tree (don't rely on auto-tag alone for complex layouts/columns).
- **Alt text** — every meaningful image, chart, and figure has concise, informative alt text; mark
  purely decorative images as decorative/artifact. For a data graphic, the alt text conveys the
  *point*, not "chart."
- **Tables** — use real table structure with a designated **header row** (and row headers where
  needed); no layout tables; no merged cells that break reading order.
- **Color & contrast** — body text contrast **≥ 4.5:1** (≥ 3:1 for large text/UI); **never rely on
  color alone** to convey meaning (add labels/patterns). This ties directly to the brand skill's
  contrast rule.
- **Meaningful link text** — links describe their destination ("Download the SSP template"), never
  "click here" or a bare URL.
- **Lists** — use real list formatting (ordered/unordered), not manual dashes/numbers.
- **Language & metadata** — set the document **language**, a real **title** in properties, and
  bookmarks for long PDFs.
- **Reading-order for multi-column / callouts** — verify callout boxes, sidebars, and action captions
  land in a sensible spot in the tag order.
- **No scanned-image text** — text must be real text (OCR'd if scanned); forms use proper form fields
  with labels.

## VPAT / ACR

When a solicitation asks how your ICT conforms, you produce a **VPAT** (Voluntary Product Accessibility
Template) → completed, it's an **Accessibility Conformance Report (ACR)**. Use the current VPAT
edition (Section 508 edition, or INT if international standards also apply). For each applicable
criterion, state **Supports / Partially Supports / Does Not Support / Not Applicable** with an honest
remarks/explanation. Don't overclaim — a false "Supports" is a performance and integrity risk.

## Workflow

1. **Scope** — is 508 a deliverable requirement, a submission requirement, or both? Cite the exact
   Section L/M/SOW language.
2. **Author accessibly** — fix at the source (Word styles, alt text, table headers) before export.
3. **Export tagged** and **verify** — check tag tree, reading order, and run an accessibility check;
   remediate flags. Manual review still required (checkers catch ~a third of issues).
4. **Produce the ACR** if required; keep it honest.
5. **Hand back** a conformant file + a short conformance note for the submission.

## How this plugs into the CRM

- Runs as the **final pass** after brand styling on any federal-facing document (APMP → humanizer →
  structural-humanizer → brand → **508**).
- **Compliance agent** — 508 is a compliance requirement when the solicitation cites it; feed
  pass/fail back.
- **Proposal Builder / doc + pdf output** — bake accessible structure in at authoring time so export
  is clean, not a retrofit.

## Anti-patterns

- Treating 508 as cosmetic — it's a stated compliance/performance requirement when cited.
- Auto-tagging a complex PDF and assuming it's done (verify reading order manually).
- "Click here" links, color-only meaning, images with no/poor alt text, fake (visual-only) headings.
- Overclaiming conformance in a VPAT/ACR.
- Retrofitting accessibility at the end instead of authoring it in.
