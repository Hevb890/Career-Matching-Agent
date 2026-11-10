---
name: fetch-openings
description: Query ATS platforms (Greenhouse, Lever) and job feeds for openings matching a given field or query. Use when asked to fetch new jobs or run ingestion.
---

# Fetch Openings Skill

## Instructions

1. Read the parameters from `config.json` for target job titles, fields, and locations.
2. Execute the ingestion script using Python:
   ```bash
   python scripts/fetch_ats_jobs.py --config config.json --out data/raw_jobs.json
   ```
