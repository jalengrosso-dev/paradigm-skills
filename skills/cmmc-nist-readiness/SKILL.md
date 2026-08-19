---
name: cmmc-nist-readiness
description: >-
  Walk a client through CMMC 2.0 / NIST SP 800-171 readiness for DoD work — scoping FCI vs CUI,
  determining the required level (1/2/3), self-assessment vs C3PAO path, building the SSP and POA&M,
  the SPRS score and annual affirmation, and flow-down to subcontractors. Use whenever anyone asks
  about CMMC, cybersecurity certification for DoD contracts, NIST 800-171, DFARS 252.204-7021 or
  7012, CUI/FCI handling, SPRS score, System Security Plan, POA&M, C3PAO assessment, or "are we
  cyber-ready to bid on DoD work." Owns the CMMC readiness workflow that the compliance and risk
  agents only flag. NOTE: the CMMC rollout timeline is under active DoD review — verify live status
  before giving any date- or phase-specific advice.
---

# GovCon CMMC 2.0 / NIST 800-171 Readiness

Owns end-to-end CMMC readiness for a client. The Compliance agent *flags* whether a CMMC level is
required; the Risk agent *flags* accuracy exposure. This skill does the actual work: scope, determine
level, close gaps, produce the artifacts, and keep the client eligible to bid.

Relevance to PSS's book of business: owner-operated construction/civil-infrastructure firms doing DoD
facility or infrastructure work routinely handle **FCI** (SOWs, schedules, non-public correspondence)
and often **CUI** (technical drawings, engineering specs, test data). That pulls them — and their
subs — into CMMC scope.

## ⚠️ Live-status caveat (read first)

CMMC's rollout is a **moving regulatory target**. Anchor advice on the durable methodology below;
**verify the current phase/enforcement status before giving any date-specific guidance**, because it
has changed repeatedly.

Current status *as of Aug 2026* (confirm before advising):
- The DFARS acquisition rule (48 CFR / **DFARS 252.204-7021**) took effect **Nov 10, 2025** —
  Phase 1. Since then, DoD solicitations have carried **Level 1 (Self)** and **Level 2 (Self)**
  requirements; results go in **SPRS** with an **annual senior-official affirmation**.
- As of **July 13, 2026**, DoD **paused Phases 2–4** for a ~60-day CMMC reform review. During the
  pause, program offices may designate only **Level 1 (Self)** or **Level 2 (Self)** — **not** Level 2
  (C3PAO) or Level 3 (DIBCAC); active solicitations requiring those are being amended.
- Phase 1 self-assessment requirements remain **live and enforceable**. The underlying NIST 800-171
  obligation under **DFARS 252.204-7012** predates CMMC and is required today regardless — so **the
  readiness work is the same** whether or not third-party assessment is currently mandated.

Two rules to keep straight: **32 CFR Part 170** = the CMMC *program* (levels, scoring, affirmations,
assessment process). **48 CFR / DFARS 252.204-7021** = the *contract clause* obligating the required
level at award and flow-down. Verify both at 32 CFR §170 and current DoD/SPRS guidance.

## Step 1 — Scope: FCI vs CUI (this drives everything)

- **FCI** (Federal Contract Information) — non-public info provided by or generated for the government
  under a contract (SOWs, delivery schedules, non-public correspondence). → points to **Level 1**.
- **CUI** (Controlled Unclassified Information) — technical data, drawings, specs, source-selection
  info, export-controlled (ITAR/EAR) material, covered defense information. → points to **Level 2+**.
- Clients routinely **underestimate CUI exposure.** For construction/civil firms, treat engineering
  drawings, specifications, test results, and logistics data as likely CUI until proven otherwise;
  confirm against the contract's CUI markings and the CO. Define the **assessment boundary** (the
  systems/people/facilities that process, store, or transmit FCI/CUI) — a tight, well-drawn boundary
  is the single biggest lever on cost and effort.

## Step 2 — Determine the required level

- **Level 1 (Foundational)** — FCI only. 15 basic safeguarding requirements (FAR 52.204-21). Annual
  **self-assessment** + affirmation in SPRS.
- **Level 2 (Advanced)** — CUI. Maps exactly to **NIST SP 800-171's 110 controls** across 14 families
  (see `references/nist-800-171-families.md`). Self-assessment for some contracts; C3PAO third-party
  assessment for others (see live-status caveat).
- **Level 3 (Expert)** — most sensitive CUI. Level 2 **plus** a subset of NIST SP 800-172; assessed by
  DoD's DIBCAC.
- The level is set by the **contract/solicitation**, not by preference. Subcontractors must meet the
  level required for the FCI/CUI they handle (**flow-down per 32 CFR 170.23** and the 7021 clause).

## Step 3 — Gap assessment & scoring

- Assess the environment against the applicable control set; compute the **SPRS score** (Level 2 uses
  the NIST 800-171 DoD Assessment Methodology: start at 110, subtract weighted points for unmet
  controls — 1, 3, or 5 points each; the floor can go negative).
- **POA&M rules (Level 2/3):** conditional certification is allowed only if the score is **≥ 80%** of
  points; **3- and 5-point (higher-weighted) controls must be fully implemented** and are **not**
  POA&M-eligible; open POA&M items must be **closed within 180 days**.
- A full CMMC assessment is valid **3 years**, with an **annual affirmation** by a senior official in
  SPRS.

## Step 4 — Produce the core artifacts

1. **System Security Plan (SSP)** — documents the boundary and how each control is implemented. The
   central artifact; assessors evaluate against it.
2. **POA&M** — remediation plan for each open gap: owner, steps, milestones, close-out date (≤180 days).
3. **SPRS entry** — post the score and maintain the affirmation.
4. **Supporting policies/evidence** — the artifacts each control family expects (access control lists,
   incident-response plan, training records, config baselines, MSP/ESP agreements, etc.).

## Step 5 — Plan the path & timeline

- Readiness typically takes **6–12 months** depending on current posture; C3PAO scheduling (when
  required) takes **weeks to months**, so engage **6–9 months** before you expect to need it.
- Small firms: consider a compliant **MSP/ESP** or **enclave** to shrink the boundary and cost.
  Roughly ~73% of the DIB are small businesses — the burden is real; scope tightly and sequence
  remediation by point-weight (fix 5- and 3-point controls first — they can't be POA&M'd).
- Bidding while remediating is sometimes possible, but the required level must be met **by award**.

## How this plugs into the CRM

- **Compliance agent** flags "CMMC level required?" → hand off here for the actual readiness workflow.
- **Risk agent** — an inaccurate self-assessment/affirmation is a False Claims Act exposure; feed the
  SSP/POA&M honesty check back to it.
- **Business Readiness agent** — CMMC readiness is a Phase-4/5 (financial leverage / ecosystem) item;
  sequence it when a client targets DoD CUI work.
- **Teaming/Mentor-Protégé** — a mentor's compliant enclave can be a legitimate path for a protégé.

## Anti-patterns

- Advising specific phase/date requirements without checking live status (it's under active review).
- Assuming "we only handle FCI" without testing drawings/specs/test data for CUI.
- Treating CMMC as a one-time audit — it's continuous (annual affirmation, change notifications).
- POA&M'ing a 3- or 5-point control (not allowed) or ignoring the 80% conditional-cert floor.
- Drawing the assessment boundary too wide (cost explodes) — or too narrow to be defensible.
- Promising certification timelines that ignore C3PAO scheduling lead time.

Detail: `references/nist-800-171-families.md`.
