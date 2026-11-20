# Ridgecourse Roofing

Remote clerical support for roofing and restoration offices. The first fixed-fee pilot covers an Arizona business and an Arizona non-claim job. Other U.S. businesses can ask about future availability.

The office receives a source index, supplier records paired by supplied identifiers and a list of open items. Ridgecourse holds neither a contractor license nor an insurance adjuster license. Scope excludes construction, field supervision, estimates, property-specific weather conclusions and assignments for open or anticipated claims.

## Run the site

Serve the static directory with Python.

```sh
python3 -m http.server 8000 --directory site
```

Open `http://localhost:8000`. The two-file checklist, print view and text export run in the browser. Images and fonts are self-hosted. The photography consists of illustrative, AI-generated architectural studies.

## Publish and sync

The dedicated Vercel project publishes `site/`. The holding website mounts a pinned copy under `/roofing` and lists Ridgecourse in the portfolio. From a holding-site checkout, sync a committed source revision using the command below.

```sh
node scripts/sync-ridgecourse.mjs /path/to/ridgecourseroofing FULL_40_CHAR_COMMIT_SHA
```

[Dedicated site](https://ridgecourseroofing.summithillholdings.com/) · [Holding site](https://summithillholdings.com/roofing) · [Portfolio listing](https://summithillholdings.com/portfolio/ridgecourse-roofing)
