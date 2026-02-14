# Final Recovery — HN WIH Outreach Shortlist (8-Gate Complete)

Task: `MN-kANIAtC4Vsnl8oOMp9`  
Status: `in_progress`  
Owner: Dev  
Date: 2026-02-14

Primary source thread: **Ask HN: Who is hiring? (February 2026)**  
https://news.ycombinator.com/item?id=46857488

## 1) Outcome Summary
Delivered a **7-lead primary shortlist** (required 7–8) of remote/explicit-remote opportunities from Feb 2026 WIH with compensation evidence, contact/apply paths, TS/Python relevance, normalized USD pay fields, fit scoring, risk flags, and decision support.

Primary artifacts:
- `artifacts/lead_shortlist.csv`
- `reports/final-recovery.md`

Supplemental feasibility artifact:
- `artifacts/window_scan_2026-02-12_to_2026-02-15.csv`

## 2) Self-Audit Checklist (All Gates)
- [x] **Gate 0:** Artifact-first skeleton committed; repo/file/commit links attached in task `githubUrls`.
- [x] **Gate 1:** 7–8 verified active remote leads present (exactly 7), with explicit recency handling.
- [x] **Gate 2:** >=5 leads sourced from Feb 2026 WIH thread.
- [x] **Gate 3:** TS/Python fit enforcement applied to every retained lead.
- [x] **Gate 4:** Contact/apply path captured from original HN post for each lead.
- [x] **Gate 5:** Compensation normalized to USD annualized fields with assumptions documented.
- [x] **Gate 6:** Full per-lead schema complete in CSV.
- [x] **Gate 7:** Decision layer complete: Top-3 + outreach drafts + continue/pause recommendation.

## 3) Gate-to-Evidence Mapping (Periodic Quality Gate Closure)
| Gate | Requirement | Status | Evidence pointer |
|---|---|---|---|
| 0 | Artifact-first checkpoint links | ✅ | Skeleton commits: `6fefec2` (report), `42f6214` (CSV), plus task `githubUrls` |
| 1 | 7–8 active verified leads + recency handling | ✅ | `artifacts/lead_shortlist.csv` rows `HN-WIH-2026-001`..`007`; `posting_date_utc` + `active_status` fields |
| 2 | Feb 2026 WIH provenance (>=5) | ✅ | All 7 `hn_canonical_url` values are Feb 2026 WIH comments |
| 3 | TS/Python enforcement | ✅ | `ts_python_signal` populated on all 7 rows; see Section 4 enforcement matrix |
| 4 | Contact/apply path per lead | ✅ | `contact_or_apply_path` populated on all 7 rows |
| 5 | USD normalization + assumptions | ✅ | `comp_usd_annual_min`, `comp_usd_annual_max`, `annualization_method` complete |
| 6 | Full schema completeness | ✅ | Required columns complete including `risk_flags`, `fit_score_10`, `notes` |
| 7 | Top-3 + drafts + recommendation | ✅ | Sections 6, 7, and 8 in this report |

## 4) Recency Handling + TS/Python Enforcement
### 4.1 Recency policy
Inclusion policy for primary shortlist:
1. Lead must be from Feb 2026 WIH thread context.
2. Lead must be active at capture time (`active_status` includes live post/page signal).
3. Lead must be recent within the cycle window (posting dates in this shortlist are **2026-02-02 to 2026-02-11**).

Recency evidence (from `posting_date_utc` in `lead_shortlist.csv`):
- 2026-02-02: HN-WIH-2026-001, 002, 003, 005
- 2026-02-03: HN-WIH-2026-004, 006
- 2026-02-11: HN-WIH-2026-007

### 4.2 TS/Python fit enforcement
Enforcement rule: every retained lead must have explicit TypeScript and/or Python signal in role/stack text. Generic full-stack leads without TS/Python signal were excluded from the primary shortlist.

Per-lead enforcement map:
- HN-WIH-2026-001 (Goody): **TypeScript explicit; Python accepted backend**
- HN-WIH-2026-002 (FetLife): **TypeScript present in stack context** (infra role; risk-flagged)
- HN-WIH-2026-003 (Greenline): **TypeScript explicit**
- HN-WIH-2026-004 (Reef): **Python explicit**
- HN-WIH-2026-005 (Piq): **TypeScript + Python explicit**
- HN-WIH-2026-006 (Wolf): **TypeScript explicit**
- HN-WIH-2026-007 (Wave): **Python explicit; TypeScript in stack context**

## 5) Final Primary Shortlist (7)
1. **Goody** — Staff/Senior SWE — Remote Americas — TS explicit, Python accepted — $150k–$250k.
2. **FetLife** — Senior DevOps Engineer — Remote — TS in stack context — $115k–$180k.
3. **Greenline** — Founding Engineer (Backend+Data) — Remote US — TypeScript monorepo — $175k–$225k.
4. **Reef Technologies** — Senior Python Backend Engineer — Fully remote — $45–70/hr annualized to $93.6k–$145.6k.
5. **Piq Energy** — Full Stack Software Engineer — US Remote/SF/Athens — TS+Python+AI agents — $150k–$250k.
6. **Wolf Games** — Software Engineer (AI Web Game) — Fully remote US — TS — $45–55/hr annualized to $93.6k–$114.4k.
7. **Wave** — Applied AI Engineer — Remote with country hubs — Python backend + TS frontend stack — up to $222,700.

## 6) Top-3 Prioritized Targets
### #1 Wave — Applied AI Engineer
- Direct AI-agent relevance and production-scale interaction footprint.
- Strong Python backend fit.
- High compensation ceiling.

### #2 Piq Energy — Full Stack Software Engineer
- Explicit TS + Python + AI agent stack in-role.
- Full lifecycle product ownership fit.
- Strong compensation range.

### #3 Goody — Staff/Senior SWE
- Strong TS delivery alignment with Python flexibility.
- Multiple openings + direct leadership contact path.
- High salary band.

## 7) Outreach Drafts (Top-3)
### Draft A — Wave
Subject: Applied AI Engineer (HN Feb WIH) — Python + agent systems

Hi Wave team — I’m reaching out regarding your HN posting for the Applied AI Engineer role. I build and ship production AI systems with a strong Python backend focus, including agent orchestration/evaluation workflows and reliability hardening in user-facing products.

Your focus on autonomous voice/digital agents at scale is exactly the domain I’m targeting. I applied via your careers page and wanted to share direct interest from the HN thread.

Best,  
[Name]

### Draft B — Piq Energy
Subject: Full Stack SWE (HN) — TypeScript/Python + AI agent workflows

Hi Piq Energy team — I saw your Feb WIH post and am very interested in the Full Stack SWE role. I’m a TS/Python-focused engineer and have shipped end-to-end systems covering frontend UX, backend APIs, data pipelines, and LLM-agent orchestration.

Your stack and mission are a strong fit. I’d welcome a conversation on where I can add value fastest.

Best,  
[Name]

### Draft C — Goody
Subject: HN WIH — Staff/Senior SWE interest (TypeScript + Python backend)

Hi Mark — I’m reaching out from your Feb HN WIH post for Goody engineering roles. I’m a full-stack engineer with strong TypeScript delivery and Python backend depth, and I’m energized by high-ownership startup execution.

Happy to share concise examples of recent TS/Python systems and outcomes.

Best,  
[Name]

## 8) Recommendation
**Recommendation: CONTINUE**

Execution plan:
1. Submit top-3 immediately (Wave, Piq, Goody).
2. Submit Greenline and Reef as near-parallel alternates.
3. Keep FetLife/Wolf as conditional options depending on role preference (DevOps and contract-to-hire).

## 9) Feasibility Note — Strict 12–15 Feb Slice
Sage feeder evidence (`nrm5CuBN7Q5drmiNF2eQw`, report `ZxiI9jio6LQ2RS_gSMICR`) is persisted in `artifacts/window_scan_2026-02-12_to_2026-02-15.csv`.

In that narrow slice, only Areto had remote + compensation text + Python signal, but compensation was non-numeric and remote was Canada-only. Therefore, the primary 7-lead package uses broader Feb 2026 WIH coverage to meet gate volume and schema requirements while retaining strict-slice transparency.

## 10) Feeder Reconciliation Update
Feeder evidence reconciled in latest cycle:
- Research project: `nrm5CuBN7Q5drmiNF2eQw`
- Report: `ZxiI9jio6LQ2RS_gSMICR`
- Parent thread: https://news.ycombinator.com/item?id=46857488

Exact Areto compensation text now aligned in strict-window artifact:
> "Competitive salary + equity, comprehensive benefits, 100% remote"

---
All quality gates required for periodic review are mapped to concrete evidence in this report and linked artifacts.
