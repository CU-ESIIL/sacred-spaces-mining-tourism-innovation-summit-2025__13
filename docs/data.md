# Data access & stewardship

This page documents datasets used by the Sacred Spaces sprint. Link to shared storage locations, note any usage constraints, and flag who to contact for questions.

## Active datasets

| Dataset | Description | Access | Notes |
|---------|-------------|--------|-------|
| BLM Recreation Sites & Trails | Public land recreation features used for baseline access layers | [Recreation.gov bulk download](https://www.recreation.gov/) | Sync curated extracts to `data/blm_trails/` and CyVerse `Group_13/shared_data/` |
| Tribal Historic Preservation GIS (summary) | Confidential cultural stewardship zones aggregated for planning | Request via cultural advisors | Store generalized layers only; original sensitive data remains with partners |
| Visitor Mobility Tiles | Aggregated mobility data to identify approach patterns | Contact analytics pod | Keep raw tiles in CyVerse; publish only summarized rasters |
| Mine Closure Registry | Infrastructure attributes for reclaimed sites | [USGS Mine Closure Inventory](https://www.usgs.gov/) | Document cleaning steps in `code/data_processing.md` |

## Storage locations

- **CyVerse community folder:** [`i:/iplant/home/shared/esiil/Innovation_summit/Group_13`](https://de.cyverse.org/data/ds/iplant/home/shared/esiil/Innovation_summit/Group_13?type=folder&resourceId=c244d2a2-95a1-11f0-b0fb-90e2ba675364)
- **GitHub repo data directory:** `data/` (for small, shareable samples or derived artifacts under 50 MB).

## Data stewardship checklist

- [x] Confirm sensitive cultural datasets remain in controlled storage.
- [ ] Document data licenses and sharing agreements before final publication.
- [ ] Add metadata README files to each CyVerse subfolder.
