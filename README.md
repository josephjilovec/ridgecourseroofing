# Ridgecourse Roofing

**National B2B Roofing & Restoration Operations, Job-File Audits & Documentation Support (US · 100% Remote · Strictly Fixed-Fee).**

> **Licensing & Scope Disclosure:** Ridgecourse Roofing is **Not a Licensed Roofing Contractor & Not a Public Adjuster**. We provide strictly B2B back-office operations, photo/evidence indexing, estimate-to-invoice reconciliation, permit/COI/lien-waiver tracking, and public NOAA/NWS storm-swath event documentation to licensed roofing contractors, water-mitigation companies, fire/contents restorers, and multi-site commercial/HOA asset teams nationwide. We do not install or inspect roofs, negotiate insurance claims, represent policyholders, waive deductibles, or charge contingency/claim-percentage fees.

## What is inside `site/`

- **Four B2B Back-Office Capabilities:** Roofing Job-File & Supplement-Prep Audits, Water-Mitigation & Psychrometric Log QA, Permit/COI/Lien-Waiver & Closeout File Coordination, and Public NOAA/NWS Storm-Swath Event Intelligence.
- **6-Stage Post-Sale Back-Office Workflow & Fixed-Fee Engagement Tiers:** Transparent fixed per-file, per-batch, and monthly operational capacity structures (zero % of claim proceeds).
- **Interactive 12-Point Job-File & Scope Completeness Auditor (`File A` vs. `File B`):** Browser-local QA tool helping contractors check documentation, bare-deck/flashing photos, supplier invoices, moisture logs, permits, and lien waivers prior to final invoicing or closeout.
- **Interactive B2B Job-File Intake & Exception Prep Sheet:** Local-only checklist exporting a plain-text `.txt` or print-ready dossier (zero account, zero server submission, zero tracking).
- **Clear Legal & Operating Boundaries:** Explicit side-by-side breakdown of B2B technical assistance versus prohibited contracting or public adjusting activities.

## Run locally

```sh
python3 -m http.server 8000 --directory site
```

Open **http://localhost:8000**. Pure HTML, CSS, and vanilla JavaScript — zero external CDNs, zero build step, zero third-party trackers.

## Publish & sync

`site/` is the complete deployable static directory. It deploys directly on Vercel at [ridgecourseroofing.summithillholdings.com](https://ridgecourseroofing.summithillholdings.com) (with `rootDirectory: "site"`). The Summit Hill Holdings website also mounts a pinned snapshot at [summithillholdings.com/roofing](https://summithillholdings.com/roofing) and lists the venture at [summithillholdings.com/portfolio/ridgecourse-roofing](https://summithillholdings.com/portfolio/ridgecourse-roofing).

To refresh the mounted copy from a `summithillholdings` checkout after committing changes here:

```sh
node scripts/sync-ridgecourse.mjs /path/to/ridgecourseroofing FULL_40_CHAR_COMMIT_SHA
```

## Imagery notice

All architectural roof and workflow visuals in `site/assets/` are original AI-generated illustrative visuals. **No completed customer jobs or client files are pictured.**
