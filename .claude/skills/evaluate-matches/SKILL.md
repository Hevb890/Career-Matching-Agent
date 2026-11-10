---
name: evaluate-matches
description: Compare retrieved jobs against candidate_profile.md. Compute match scores, gap reports, and write findings to data/matched_roles.json.
---

# Evaluate Matches Skill

## Instructions

1. Load `candidate_profile.md` and read `data/raw_jobs.json`.
2. For each job posting, evaluate alignment across 4 dimensions:
   - **Core Technical Stack** (40% weight)
   - **Experience Level & Scope** (20% weight)
   - **Architectural & Systems Fit** (20% weight)
   - **Domain Knowledge & Stretch Goals** (20% weight)
3. Calculate total match score (0–100%).
4. For roles scoring **>= 75%**, compile a breakdown:
   - **Strengths/Exact Fits**
   - **Skill Gaps / Keywords to Emphasize**
   - **Suggested CV Adjustments**
5. Write or update structured results into `data/matched_roles.json`.
