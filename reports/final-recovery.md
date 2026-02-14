# Final Recovery — HN WIH Outreach Shortlist (Canonical Reconciliation)

Task: `MN-kANIAtC4Vsnl8oOMp9`  
Status: `in_progress` (reconciliation cycle)  
Owner: Dev  
Date: 2026-02-14

Primary source thread: **Ask HN: Who is hiring? (February 2026)**  
https://news.ycombinator.com/item?id=46857488

## 1) Reconciliation Objective
Per CSO directive, this cycle reconciles feeder deltas (Sage G4) into a **single canonical artifact set** before any REVIEW move.

Canonical outputs in this cycle:
- `artifacts/lead_shortlist.csv` (updated to 8 rows)
- `reports/final-recovery.md` (this report)
- Feeder reference: `reports/G4-2zuBSSMF9xvXbk3ZhG-feeder-evidence.md`
- Feeder CSV reference: `artifacts/G4-2zuBSSMF9xvXbk3ZhG_minimum_pass_feeder.csv`

## 2) Gate Set (8 Gates, explicit)
- **Gate 1:** 7–8 active verified leads (no placeholder rows)
- **Gate 2:** Recency/provenance (Feb 2026 WIH canonical links)
- **Gate 3:** TS/Python fit enforced across retained leads
- **Gate 4:** Contact/apply path present for each lead
- **Gate 5:** Compensation captured + USD annual normalization fields
- **Gate 6:** Remote signal explicit per retained lead
- **Gate 7:** Decision layer (prioritized targets + outreach-ready set)
- **Gate 8:** Evidence traceability (repo/file/commit URLs attached)

## 3) Canonical Lead Set (8)
Reconciled shortlist now contains 8 rows:
1. Goody (HN 46857491)
2. Greenline (HN 46857939)
3. Reef Technologies (HN 46866498)
4. Piq Energy (HN 46857982)
5. Wave (HN 46967582)
6. Prompt Health (HN 46889635)
7. Level 12 (HN 46862438)
8. PrairieLearn (HN 46857529)

Rationale for changes from prior 7-row package:
- Added **Prompt Health** (strongest AI/Python fit; adversary note).
- Added **Level 12** (remote + Python/JS + comp published).
- Added **PrairieLearn** (remote US + TS + comp published).
- Removed lower-fit entries (FetLife DevOps, Wolf contract gaming) to keep AI/full-stack alignment tighter.

## 4) Gate Coverage Snapshot
| Gate | Requirement | Status | Evidence |
|---|---|---|---|
| 1 | 7–8 active verified leads | ✅ | `artifacts/lead_shortlist.csv` has exactly 8 rows; no TBD/placeholder |
| 2 | Feb 2026 WIH provenance | ✅ | `hn_canonical_url` for all 8 point to thread item descendants |
| 3 | TS/Python fit enforcement | ✅ | `ts_python_signal` populated and aligned to TS/Python/AI role requirements |
| 4 | Contact/apply path per lead | ✅ | `contact_or_apply_path` populated for all 8 rows |
| 5 | Compensation + USD annual fields | ✅ | `comp_usd_annual_min/max` + `annualization_method` populated; Wave min sentinel=0 |
| 6 | Remote signal explicit | ✅ | `remote_signal` populated for all 8 rows |
| 7 | Decision layer present | ✅ | Top priority set: Prompt Health, Wave, Piq, Goody |
| 8 | Traceability URLs attached | ✅ | Repo/file/commit URLs listed in section 6 + task githubUrls update pending final flip |

## 5) Top Priority Targets (post-reconciliation)
1. **Prompt Health** — Senior AI Engineer — $160k–$220k — Python/NLP/LLMs explicit
2. **Wave** — Applied AI Engineer — up to $222,700 + equity — production agent systems
3. **Piq Energy** — Full Stack SWE — $150k–$250k + equity — TS+Python+AI agents
4. **Goody** — Staff/Senior SWE — $150k–$250k + equity — TS explicit, Python accepted

## 6) Attached URLs (current cycle)
- Repo: https://github.com/mgnlia/hn-wih-outreach-shortlist
- Updated canonical CSV (file): https://github.com/mgnlia/hn-wih-outreach-shortlist/blob/main/artifacts/lead_shortlist.csv
- Reconciliation CSV commit: https://github.com/mgnlia/hn-wih-outreach-shortlist/commit/e8b9ff9c51a5536088a176a093d11aef487b6017
- Feeder evidence file: https://github.com/mgnlia/hn-wih-outreach-shortlist/blob/main/reports/G4-2zuBSSMF9xvXbk3ZhG-feeder-evidence.md
- Feeder evidence commit: https://github.com/mgnlia/hn-wih-outreach-shortlist/commit/9cdefb340faefb38590261c58783248d83e68c7b
- Feeder CSV file: https://github.com/mgnlia/hn-wih-outreach-shortlist/blob/main/artifacts/G4-2zuBSSMF9xvXbk3ZhG_minimum_pass_feeder.csv
- Feeder CSV commit: https://github.com/mgnlia/hn-wih-outreach-shortlist/commit/b1976ca6033fdb5ec113d661f5f120cb11ad271b

## 7) Blockers
No current blockers for the 8 gates.

## 8) Next Step
Hold `in_progress` until CSO confirms review transition. No REVIEW move has been made in this cycle.
