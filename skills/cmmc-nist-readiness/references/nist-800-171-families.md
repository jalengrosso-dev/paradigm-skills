# NIST SP 800-171 Control Families (CMMC Level 2)

CMMC **Level 2** requires all **110 security requirements** of NIST SP 800-171, organized into **14
families**. Use this to structure the SSP, the gap assessment, and the POA&M. Requirement counts are
the standard Rev 2 distribution (the baseline the DoD Assessment Methodology scores against); confirm
the exact revision cited in the client's contract, as **Rev 3** is being adopted over time and
renumbers/adjusts some requirements.

> Scoring note: the DoD Assessment Methodology starts at 110 and subtracts **1, 3, or 5 points** per
> unmet requirement by risk weight. Conditional certification needs **≥ 80%**; **3- and 5-point
> controls cannot be POA&M'd**; open items close within **180 days**.

## The 14 families

1. **Access Control (AC)** — limit system access to authorized users, processes, and devices; enforce
   least privilege, separation of duties, remote-access controls, and session lock. (Largest family.)
2. **Awareness & Training (AT)** — security awareness for all users; role-based training for
   privileged and security roles; insider-threat awareness.
3. **Audit & Accountability (AU)** — create, protect, and retain audit logs; ensure actions are
   traceable to individual users; time-synchronized, reviewed logs.
4. **Configuration Management (CM)** — baseline configurations, change control, least-functionality,
   allow/deny-listing of software, inventory of components.
5. **Identification & Authentication (IA)** — uniquely identify users/devices; **multifactor
   authentication** for network and privileged access; password/authenticator management.
6. **Incident Response (IR)** — operational IR capability: preparation, detection, analysis,
   containment, recovery, reporting; test the IR plan.
7. **Maintenance (MA)** — controlled system maintenance; sanitize equipment before off-site
   maintenance; supervise maintenance personnel.
8. **Media Protection (MP)** — protect, mark, and sanitize media containing CUI (digital and paper);
   control removable media; encrypt CUI on media.
9. **Personnel Security (PS)** — screen individuals before granting CUI access; protect CUI during
   personnel transfers and terminations.
10. **Physical Protection (PE)** — limit physical access to systems and facilities; escort/monitor
    visitors; protect and monitor the physical facility and alternate work sites.
11. **Risk Assessment (RA)** — periodically assess risk; **scan for vulnerabilities** and remediate;
    (Rev 3 adds supply-chain risk considerations).
12. **Security Assessment (CA)** — assess controls, develop and maintain the **SSP** and **POA&M**,
    monitor controls on an ongoing basis.
13. **System & Communications Protection (SC)** — boundary protection, encryption of CUI in transit
    and at rest, network segmentation, deny-by-default. (Second-largest family.)
14. **System & Information Integrity (SI)** — flaw remediation/patching, malicious-code protection,
    monitoring and alerts, respond to indicators.

## Practical remediation order for a small construction/civil firm

1. **Identify & scope** the boundary; confirm CUI vs FCI on real project documents (drawings, specs).
2. **Knock out the high-weight, non-POA&M-able controls first** — commonly **MFA (IA)**, **encryption
   of CUI in transit/at rest (SC)**, **audit logging (AU)**, **FIPS-validated crypto**, and
   **boundary protection (SC)**.
3. **Stand up the governing artifacts** — SSP first (you can't be assessed without it), then the
   policies/procedures each family expects, then evidence collection.
4. **Consider an enclave or a compliant MSP/ESP** to keep CUI in a small, well-controlled boundary
   rather than hardening the entire company network.
5. **Build the POA&M** for what remains, sequence by point-weight and 180-day close-out, and post the
   **SPRS** score with the senior-official affirmation.

## Common CUI triggers in construction/civil GovCon
Engineering drawings and specifications, geotechnical/test data, facility security details, site
plans for controlled facilities, export-controlled technical data (ITAR/EAR), and source-selection or
proposal information marked CUI. When in doubt, treat as CUI and confirm with the CO and the
contract's CUI markings.
