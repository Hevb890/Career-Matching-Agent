# Career Matching Agent - Claude Code Workspace

## Project Purpose

Autonomously monitor, extract, score, and report job openings across target technology fields (AI Engineering, Multi-Agent Systems, Microservices Architecture, Data Engineering, Software Engineering, AI/ML Engineering, Computational Social Science).

## Key Paths & Files

- Candidate Profile: `candidate_profile.md`
- Configuration File: `config.json`
- Output Folder: `data/`
- Custom Skills: `.claude/skills/`

## Operational Guardrails & Rules

1. **Filtering Standard**: Ignore job postings older than 14 days or those requiring on-site presence if the target is remote/hybrid.
2. **Match Threshold**: Require a minimum match score of 75% before flagging a job opening in `data/matched_roles.json`.
3. **Execution Isolation**: Store raw API payloads in `data/raw_jobs.json` before processing. Do not overwrite existing match logs; append with timestamps.
4. **Data Hygiene**: Always output clean, valid, indented JSON without inline comment tags.
