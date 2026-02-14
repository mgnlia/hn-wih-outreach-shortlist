# Final Recovery — HN WIH Outreach Shortlist (9-Gate Complete)

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

## 2) Gate Definitions (Current Cycle: 9 Gates)
- **Gate 0:** Artifact-first skeleton committed with repo/file/commit links in task.
- **Gate 1:** 7–8 verified active leads.
- **Gate 2:** Recency handling/validation documented and evidenced.
- **Gate 3:** Feb 2026 WIH provenance (>=5 leads).
- **Gate 4:** TS/Python fit enforcement.
- **Gate 5:** Contact/apply path captured for each lead.
- **Gate 6:** Compensation normalization to USD annual fields with assumptions.
- **Gate 7:** Decision layer complete (Top-3 + outreach drafts + continue/pause recommendation).
- **Gate 8:** Self-audit table mapping each gate to exact evidence location.

## 3) Self-Audit Checklist (All Gates)
- [x] Gate 0 complete
- [x] Gate 1 complete
- [x] Gate 2 complete
- [x] Gate 3 complete
- [x] Gate 4 complete
- [x] Gate 5 complete
- [x] Gate 6 complete
- [x] Gate 7 complete
- [x] Gate 8 complete

## 4) Self-Audit Table — Gate → Evidence Location
| Gate | Requirement | Status | Evidence location |
|---|---|---|---|
| 0 | Artifact-first checkpoint links | ✅ | Task `githubUrls`; skeleton commits `6fefec2` (report), `42f6214` (CSV) |
| 1 | 7–8 active verified leads | ✅ | `artifacts/lead_shortlist.csv` rows `HN-WIH-2026-001`..`007`; `active_status` column |
| 2 | Recency validation | ✅ | `artifacts/lead_shortlist.csv` `posting_date_utc` (2026-02-02..2026-02-11); Section 5.1 in this report |
| 3 | Feb 2026 WIH provenance >=5 | ✅ | `artifacts/lead_shortlist.csv` `hn_canonical_url` on all 7 rows (all Feb WIH thread) |
| 4 | TS/Python fit enforcement | ✅ | `artifacts/lead_shortlist.csv` `ts_python_signal`; Section 5.2 enforcement map |
| 5 | Contact/apply path per lead | ✅ | `artifacts/lead_shortlist.csv` `contact_or_apply_path` complete on all rows |
| 6 | USD compensation normalization | ✅ | `artifacts/lead_shortlist.csv` `comp_usd_annual_min/max` + `annualization_method` |
| 7 | Top-3 + drafts + recommendation | ✅ | Sections 7, 8, 9 in this report |
| 8 | In-file gate mapping table | ✅ | Section 4 (this table) |

## 5) Enforcement Notes
### 5.1 Recency handling
Inclusion policy for primary shortlist:
1. Lead must be from Feb 2026 WIH thread context.
2. Lead must be active at capture time (`active_status` indicates live post/page signal).
3. Lead must be recent in-cycle.

Recency evidence from CSV:
- 2026-02-02: HN-WIH-2026-001, 002, 003, 005
- 2026-02-03: HN-WIH-2026-004, 006
- 2026-02-11: HN-WIH-2026-007

### 5.2 TS/Python fit enforcement
Rule: each retained lead must include explicit TypeScript and/or Python signal.

Per-lead enforcement map:
- HN-WIH-2026-001 (Goody): TypeScript explicit; Python accepted backend
- HN-WIH-2026-002 (FetLife): TypeScript in stack context (infra role)
- HN-WIH-2026-003 (Greenline): TypeScript explicit
- HN-WIH-2026-004 (Reef): Python explicit
- HN-WIH-2026-005 (Piq): TypeScript + Python explicit
- HN-WIH-2026-006 (Wolf): TypeScript explicit
- HN-WIH-2026-007 (Wave): Python explicit; TypeScript in stack context

## 6) Final Primary Shortlist (7)
1. **Goody** — Staff/Senior SWE — Remote Americas — TS explicit, Python accepted — $150k–$250k.
2. **FetLife** — Senior DevOps Engineer — Remote — TS in stack context — $115k–$180k.
3. **Greenline** — Founding Engineer (Backend+Data) — Remote US — TypeScript monorepo — $175k–$225k.
4. **Reef Technologies** — Senior Python Backend Engineer — Fully remote — $45–70/hr annualized to $93.6k–$145.6k.
5. **Piq Energy** — Full Stack Software Engineer — US Remote/SF/Athens — TS+Python+AI agents — $150k–$250k.
6. **Wolf Games** — Software Engineer (AI Web Game) — Fully remote US — TS — $45–55/hr annualized to $93.6k–$114.4k.
7. **Wave** — Applied AI Engineer — Remote with country hubs — Python backend + TS frontend stack — up to $222,700.

## 7) Top-3 Prioritized Targets
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

## 8) Outreach Drafts (Top-3)
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

## 9) Recommendation
**Recommendation: CONTINUE**

Execution plan:
1. Submit top-3 immediately (Wave, Piq, Goody).
2. Submit Greenline and Reef as near-parallel alternates.
3. Keep FetLife/Wolf as conditional options depending on role preference (DevOps and contract-to-hire).

## 10) Feasibility Note — Strict 12–15 Feb Slice
Sage feeder evidence (`nrm5CuBN7Q5drmiNF2eQw`, report `ZxiI9jio6LQ2RS_gSMICR`) is persisted in `artifacts/window_scan_2026-02-12_to_2026-02-15.csv`.

In that narrow slice, only Areto had remote + compensation text + Python signal, but compensation was non-numeric and remote was Canada-only. Therefore, the primary 7-lead package uses broader Feb 2026 WIH coverage to meet gate volume and schema requirements while retaining strict-slice transparency.

## 11) Evidence-Gap Section (Feeder Timeout Rule)
**Rule used:** if feeder is delayed beyond 30 minutes, proceed with available verified data and log gaps explicitly.

Current status in this cycle:
- No blocking feeder delay at finalization time; package completed from verified in-repo and persisted feeder artifacts.
- Residual evidence gap (market/data, not process): strict 12–15 Feb slice lacks numeric compensation for remote TS/Python engineering leads.
- Impact: primary deliverable is satisfied using broader Feb 2026 WIH scope; strict-slice artifact retained for transparency.

---
All 9 gates are evidenced in-file and linked to committed artifacts. Status intentionally remains `in_progress` pending explicit instruction to move `review`.
