---
name: cui-data-handling
description: >-
  Day-to-day handling of Controlled Unclassified Information (CUI) and FCI — identifying and marking
  CUI, lawful storage/transmission/encryption, email and file-share practices, subcontractor
  flow-down, incident reporting, destruction, and decontrol. Use whenever anyone asks how to mark,
  store, email, share, or destroy CUI/FCI, about CUI banner/portion markings, the CUI Registry,
  DFARS 252.204-7012 safeguarding or 72-hour incident reporting, FIPS-validated encryption for CUI, or
  "can we send this drawing to our sub." The operational companion to the CMMC readiness skill — CMMC
  proves you *can* protect CUI; this governs how you actually handle it every day.
---

# GovCon CUI / FCI Data Handling

Operational, day-to-day handling of government information. The **CMMC readiness** skill gets a client
*certified to* protect CUI; this skill governs the everyday practices that keep them compliant and out
of trouble. Especially relevant for construction/civil firms, where drawings, specs, and test data are
frequent CUI.

## Know what you're holding

- **FCI** — non-public information provided by/generated for the government under a contract (SOWs,
  schedules, non-public correspondence). Basic safeguarding (FAR 52.204-21); do not post publicly.
- **CUI** — information the government requires be protected or controlled, defined by the **NARA CUI
  Registry** and **32 CFR Part 2002**. Common construction/civil triggers: engineering drawings,
  specifications, geotechnical/test data, site/facility security details, source-selection info,
  export-controlled technical data (ITAR/EAR). **CUI//SP-** categories (e.g., export control) carry
  extra limits.
- When unsure, treat as CUI and confirm against the **contract's CUI markings** and the CO. The
  government (or prime) is responsible for designating CUI; you're responsible for protecting what's
  marked or reasonably identifiable.

## Marking (get this right — mismarking is its own problem)

- **Banner marking** at top (and bottom) of each page: `CUI` (or `CONTROLLED`), with the category and
  dissemination controls when applicable (e.g., `CUI//SP-EXPT//...`).
- **Portion marking** when required by the designating agency: `(CUI)` at the start of the controlled
  paragraph/element.
- **Designation indicator** identifying the source/authority and a point of contact.
- Do **not** over-mark (marking non-CUI as CUI causes handling burden and confusion) or under-mark.
  Decontrol only per the designating agency's instructions.

## Storing, transmitting, handling

- **Encrypt CUI at rest and in transit** with **FIPS 140-validated** cryptography (this is a
  high-weight CMMC control, not optional).
- **Email:** send CUI only over encrypted channels/portals to authorized recipients on a
  need-to-know basis; no CUI to personal accounts; mark the message; watch auto-forwarding rules.
- **File shares / cloud:** store CUI only in the assessed **boundary/enclave** (a compliant GCC High
  or equivalent, or an on-prem enclave); keep it out of general company drives. Cloud services storing
  CUI must meet **FedRAMP Moderate (or equivalent)** and the DFARS 7012 cloud requirements.
- **Access:** need-to-know + least privilege; MFA; log access. Physical CUI (printed drawings) stays
  in controlled areas and is marked, stored, and destroyed like digital CUI.
- **Removable media / mobile:** encrypt; control and inventory; avoid where possible.

## Subcontractor flow-down

- Flow **DFARS 252.204-7012** and the applicable **CMMC level (per 32 CFR 170.23 / DFARS 7021)** to
  any sub that will process, store, or transmit the FCI/CUI. The sub must meet the level required for
  what *they* handle.
- Share CUI with a sub only after the flow-down is in place and the sub is authorized; transmit through
  protected channels; track who has what.

## Incident reporting (fast clock)

- Under **DFARS 252.204-7012**, report a cyber incident affecting CUI (or the contractor's ability to
  perform) to DoD via **DIBNet within 72 hours** of discovery. Preserve/image affected systems and
  media; cooperate with any DoD damage assessment. Know this clock **before** an incident — it's tight.

## Destruction & decontrol

- Destroy CUI so it can't be reconstructed (shredding/wiping to NIST 800-88 media-sanitization
  standards). Decontrol only when the designating agency authorizes it, then remove markings and note
  the decontrol.

## How this plugs into the CRM

- **CMMC readiness** — this is the operational layer under the certification; feed real handling gaps
  into the SSP/POA&M.
- **Teaming/Contract Lifecycle** — trigger flow-down and channel setup before any CUI moves to a sub.
- **Compliance/Risk** — mismarking, personal-email leakage, and missed 72-hour reporting are the
  common failures; flag them.

## Anti-patterns

- Emailing a "drawing" to a sub before flow-down and a protected channel exist.
- CUI on general company drives / personal accounts / unencrypted media.
- Over- or under-marking; decontrolling without authority.
- Not knowing the **72-hour** DIBNet clock until an incident is underway.
- Assuming a generic commercial cloud is fine for CUI (needs FedRAMP-Mod-equivalent + 7012 terms).
