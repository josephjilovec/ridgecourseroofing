# Ridgecourse Roofing

Ridgecourse is a remote B2B operations desk for licensed roofing and restoration contractors across the United States. It organizes post-sale job records, source-linked photo indexes, supplier and subcontractor references, daily-log completeness, permit/vendor closeout lists and regional NOAA/NWS storm reports. The contractor keeps every field, technical, billing and insurance decision.

Ridgecourse holds no roofing/general-contractor or insurance-adjuster license. U.S.-wide inquiries are welcome; an engagement proceeds only after its jurisdictions, purpose, data route and scope are screened. The initial offer is internal non-claim office work. Supplement preparation, carrier-ready packets and other claim-specific assignments remain unavailable pending activity-specific legal review. Prices are fixed per file, batch or monthly office capacity, never a share of claim proceeds or recovery.

## Run the site

Serve the static directory with Python:

```sh
python3 -m http.server 8000 --directory site
```

Open `http://localhost:8000`. The 12-point two-file checklist, print view and text export run in the browser. Images and fonts are self-hosted. Architectural photography is illustrative and AI-generated; no completed customer project is depicted.

## Publish and sync

The dedicated Vercel project publishes `site/`. The Summit Hill Holdings site mounts a pinned copy under `/roofing` and lists Ridgecourse in the portfolio. From a holding-site checkout, run:

```sh
node scripts/sync-ridgecourse.mjs /path/to/ridgecourseroofing FULL_40_CHARACTER_COMMIT_SHA
```

[Dedicated site](https://ridgecourseroofing.summithillholdings.com/) · [Mounted copy](https://summithillholdings.com/roofing) · [Portfolio listing](https://summithillholdings.com/portfolio/ridgecourse-roofing)
