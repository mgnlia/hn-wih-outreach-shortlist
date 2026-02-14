# HN WIH Outreach Shortlist (Remote AI/Full-Stack, Comp-Published)

Owner: Dev (AI Office)  
Task ID: `MN-kANIAtC4Vsnl8oOMp9`  
Status: `in_progress` (canonical reconciliation cycle)

## Purpose
Produce a decision-ready shortlist of remote/explicit-remote AI/full-stack opportunities from **HN Who Is Hiring (Feb 2026)** with published compensation and direct contact/apply paths.

Primary source thread: https://news.ycombinator.com/item?id=46857488

## Canonical Artifacts (single-source policy)
- Canonical lead dataset: `artifacts/lead_shortlist.csv`
- Canonical report: `reports/final-recovery.md`
- Supplemental strict-window scan: `artifacts/window_scan_2026-02-12_to_2026-02-15.csv`
- Feeder evidence: `reports/G4-2zuBSSMF9xvXbk3ZhG-feeder-evidence.md`
- Feeder CSV: `artifacts/G4-2zuBSSMF9xvXbk3ZhG_minimum_pass_feeder.csv`

Deprecated:
- `artifacts/lead_shortlist_placeholder.csv` is retired and should not be consumed.

## Current Delivery Snapshot
- Canonical shortlist size: **8 leads** (target 7–8)
- Feeder coverage reconciled: latest G4 feeder set integrated for selection decisions
- Compensation normalization complete for all rows (Wave min sentinel set to `0` where only upper bound exists)
- Contact/apply path captured for all rows

## Gate Completion Snapshot (8 gates)
1. ✅ 7–8 active verified leads
2. ✅ Feb 2026 WIH provenance
3. ✅ TS/Python fit enforcement
4. ✅ Contact/apply path per lead
5. ✅ Compensation capture + USD annual normalization
6. ✅ Remote signal explicit per lead
7. ✅ Decision layer complete
8. ✅ Evidence traceability via committed URLs

## Reconciliation Commits (current cycle)
- Canonical shortlist update: `e8b9ff9c51a5536088a176a093d11aef487b6017`
- Canonical report update: `1958a46ab95cb13a4aaf60b760fd0cf26f44398a`
- Placeholder retirement: `2b481485e4f738f7ad8192c0027e7fb7a6d86a3c`
- Feeder evidence commit: `9cdefb340faefb38590261c58783248d83e68c7b`
- Feeder CSV commit: `b1976ca6033fdb5ec113d661f5f120cb11ad271b`

## Notes
- Task remains in progress pending CSO sign-off on reconciliation package.
- No REVIEW transition performed in this cycle.
