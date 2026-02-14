# Final Recovery — HN WIH Outreach Shortlist (Canonical Reconciliation)

Task: `MN-kANIAtC4Vsnl8oOMp9`  
Status: `in_progress` (checkpointed reconciliation cycle)  
Owner: Dev  
Date: 2026-02-14

Primary source thread: **Ask HN: Who is hiring? (February 2026)**  
https://news.ycombinator.com/item?id=46857488

## 1) Objective
Deliver a single canonical artifact set reconciled against feeder dependency `G4-2zuBSSMF9xvXbk3ZhG`, without moving to REVIEW until all 8 gates are satisfied from committed evidence.

Canonical outputs:
- `artifacts/lead_shortlist.csv`
- `reports/final-recovery.md` (this report)

Feeder references:
- `reports/G4-2zuBSSMF9xvXbk3ZhG-feeder-evidence.md`
- `artifacts/G4-2zuBSSMF9xvXbk3ZhG_minimum_pass_feeder.csv`

## 2) Verified Feeder Baseline + Delta Note
Verified feeder baseline used for reproducibility:
- Feeder evidence commit: `9cdefb340faefb38590261c58783248d83e68c7b`
- Feeder CSV commit: `b1976ca6033fdb5ec113d661f5f120cb11ad271b`

Delta note (non-blocking):
- Upstream feeder iterations include additional rows beyond the 12-lead baseline in some `main` revisions.
- This package proceeds with the verified baseline plus direct HN verification for any retained rows; no gate is blocked by feeder drift.

## 3) Gate Set (8 Gates)
- **Gate 1:** 7–8 active verified leads (no placeholders)
- **Gate 2:** Feb-2026 WIH provenance (canonical HN links)
- **Gate 3:** TS/Python fit enforced
- **Gate 4:** Contact/apply path present for each row
- **Gate 5:** Compensation captured + USD annual normalization
- **Gate 6:** Remote signal explicit for each row
- **Gate 7:** Decision layer present (priority targets)
- **Gate 8:** Evidence traceability (repo/file/commit URLs)

## 4) T+60 Gate Matrix Draft (Committed Evidence)
| Gate | Requirement | Status | Committed evidence |
|---|---|---|---|
| 1 | 7–8 active verified leads | ✅ | `artifacts/lead_shortlist.csv` contains exactly 8 rows, no TBD/placeholder entries |
| 2 | Feb-2026 WIH provenance | ✅ | `hn_canonical_url` populated for all rows with WIH thread descendant item links |
| 3 | TS/Python fit enforcement | ✅ | `ts_python_signal` field populated for all rows, aligned to role scope |
| 4 | Contact/apply path | ✅ | `contact_or_apply_path` populated for all rows |
| 5 | Compensation + USD normalization | ✅ | `comp_usd_annual_min/max` + `annualization_method` complete; Wave min sentinel normalized to `0` |
| 6 | Explicit remote signal | ✅ | `remote_signal` populated for all rows |
| 7 | Decision layer | ✅ | Priority set documented (Prompt Health, Wave, Piq, Goody) |
| 8 | Traceability URLs | ✅ | URLs listed in section 6 of this report + task `githubUrls` |

## 5) Canonical Lead Set (8)
1. Goody (HN 46857491)
2. Greenline (HN 46857939)
3. Reef Technologies (HN 46866498)
4. Piq Energy (HN 46857982)
5. Wave (HN 46967582)
6. Prompt Health (HN 46889635)
7. Level 12 (HN 46862438)
8. PrairieLearn (HN 46857529)

## 6) URL Traceability Bundle
- Repo: https://github.com/mgnlia/hn-wih-outreach-shortlist
- Canonical CSV file: https://github.com/mgnlia/hn-wih-outreach-shortlist/blob/main/artifacts/lead_shortlist.csv
- Canonical report file: https://github.com/mgnlia/hn-wih-outreach-shortlist/blob/main/reports/final-recovery.md
- Feeder evidence file: https://github.com/mgnlia/hn-wih-outreach-shortlist/blob/main/reports/G4-2zuBSSMF9xvXbk3ZhG-feeder-evidence.md
- Feeder CSV file: https://github.com/mgnlia/hn-wih-outreach-shortlist/blob/main/artifacts/G4-2zuBSSMF9xvXbk3ZhG_minimum_pass_feeder.csv
- Reconciliation CSV commit: https://github.com/mgnlia/hn-wih-outreach-shortlist/commit/e8b9ff9c51a5536088a176a093d11aef487b6017
- Feeder evidence commit: https://github.com/mgnlia/hn-wih-outreach-shortlist/commit/9cdefb340faefb38590261c58783248d83e68c7b
- Feeder CSV commit: https://github.com/mgnlia/hn-wih-outreach-shortlist/commit/b1976ca6033fdb5ec113d661f5f120cb11ad271b

## 7) Blockers
None. All 8 gates are currently satisfied from committed artifacts.

## 8) Next Step
Remain `in_progress` pending CSO evidence verification and explicit transition instruction.
