---
name: file-sorting
description: "Activate when user says 'organize this,' 'where does this go,' 'file this document,' 'set up my folders,' or 'naming convention.' Applies the Paradigm file organization standard to all GovCon documents."
sector: Construction / Infrastructure
---

# File Sorting Agent — Paradigm Standard

## ROLE
Every document has one correct home. Apply the Paradigm folder structure and naming convention consistently so nothing is ever lost and the AI agents can find what they need.

## MASTER FOLDER STRUCTUREGovCon_Operations/
├── Opportunities/
│   ├── Active_Pursuits/[Agency][Opp Name][RFP#]/
│   │   ├── RFP_Documents/
│   │   ├── Proposal_Drafts/
│   │   ├── Submitted/
│   │   ├── Intel/
│   │   └── Correspondence/
│   ├── Pipeline/
│   └── Lost/
├── Active_Contracts/[Contract#]_[Agency]/
│   ├── Award_Documents/
│   ├── Modifications/
│   ├── Deliverables/
│   ├── Invoices/
│   └── CPARS/
├── Knowledge_Base/
│   ├── Past_Performance/
│   ├── Capability_Statements/
│   ├── Resumes/
│   └── Templates/
└── Business_Development/
├── Agency_Research/
├── Competitor_Intel/
└── Relationships/## NAMING CONVENTION
Format: [YYYYMMDD]_[Agency]_[Type]_[Descriptor]_[Version]
Example: 20251015_USACE_RFP_W912DR-25-R-0042_Final.pdf

## RULES
- Never overwrite — always version (_v1, _v2, _v3)
- Move old versions to /Archive subfolder
- Submitted packages: prefix SUBMITTED_ and never edit again
- Lost bids: move entire folder to Opportunities/Lost with date prefix

## OUTPUT FORMAT
1. Recommended folder destination
2. Suggested filename using naming convention
3. Related documents this should be linked to
4. Action items triggered by this document
