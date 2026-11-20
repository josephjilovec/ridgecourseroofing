# Ridgecourse Roofing

A Phoenix & East Valley residential roofing field manual, interactive 12-point proposal scope auditor, and homeowner visit worksheet from a **Summit Hill Holdings** venture in pre-launch.

> **Arizona Licensing Notice:** Ridgecourse Roofing is currently in pre-launch and is **Not a Licensed Contractor**. Roofing inspections for hire, written contracting bids, and construction services will not open until an active **Arizona Registrar of Contractors (AZ ROC) R-42 or CR-42** license is issued, bonded, and insured.

## What is inside `site/`

- **Phoenix Desert Roof Systems Guide:** Four high-resolution architectural studies covering Clay & Concrete Tile, Underlayment & Valley Flashing Assemblies, Architectural Asphalt Shingles, and Low-Slope / SPF Foam & Parapet Roofs.
- **6-Layer Roof Anatomy & Monsoon Calendar:** Layer-by-layer breakdown of how Arizona residential roofs shed water and age under 150°F+ summer deck temperatures.
- **Interactive 12-Point Proposal Scope Auditor (`Bid A` vs. `Bid B`):** Compare two written contractor estimates side-by-side locally in your browser to highlight missing scope lines, undisclosed wood decking charges, or missing permit/lien-waiver terms.
- **Homeowner Visit Notes Worksheet:** Local-only checklist that exports a clean `.txt` file or print-ready dossier (no account, no server submission, no browser storage, zero tracking).
- **Pre-Launch Readiness & Partner Track:** Transparent milestone status covering brand clearance, operating standards, AZ ROC licensing gates, and Qualifying Party / trade supplier inquiries.

## Run locally

```sh
python3 -m http.server 8000 --directory site
```

Open **http://localhost:8000**. Pure HTML, CSS, and vanilla JavaScript — zero external CDNs, zero build step, zero third-party analytics.

## Publish & sync with Summit Hill Holdings

`site/` is the complete deployable static directory. It deploys directly on Vercel at [ridgecourseroofing.summithillholdings.com](https://ridgecourseroofing.summithillholdings.com) (and `https://ridgecourseroofing.vercel.app/`, with `rootDirectory: "site"`). The Summit Hill Holdings website also mounts a pinned snapshot at [summithillholdings.com/roofing](https://summithillholdings.com/roofing) and lists the venture at [summithillholdings.com/portfolio/ridgecourse-roofing](https://summithillholdings.com/portfolio/ridgecourse-roofing).

To refresh the mounted copy from a `summithillholdings` checkout after committing changes here:

```sh
node scripts/sync-ridgecourse.mjs /path/to/ridgecourseroofing FULL_40_CHAR_COMMIT_SHA
```

## Imagery & brand notice

All roof photographs and architectural visuals in `site/assets/` are original AI-generated illustrative visuals depicting Phoenix/Sonoran Desert roofing assemblies and materials. **No completed customer projects are pictured.** Responsive WebP/JPEG assets and the self-hosted Barlow Condensed display font (OFL notice included under `site/assets/`) keep page loads independent of third-party hosts.
