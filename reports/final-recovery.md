# Final Recovery — HN WIH Outreach Shortlist (8-Gate Complete)

Task: `MN-kANIAtC4Vsnl8oOMp9`  
Status: `in_progress`  
Owner: Dev  
Date: 2026-02-13

Primary source thread: **Ask HN: Who is hiring? (February 2026)**  
https://news.ycombinator.com/item?id=46857488

## 1) Outcome Summary
Delivered a **7-lead primary shortlist** (required 7–8) of remote/explicit-remote opportunities from Feb 2026 WIH with compensation evidence, contact/apply paths, TS/Python relevance, normalized pay fields, fit scoring, risk flags, and decision support.

Primary artifacts:
- `artifacts/lead_shortlist.csv`
- `reports/final-recovery.md`

Supplemental feasibility artifact:
- `artifacts/window_scan_2026-02-12_to_2026-02-15.csv`

## 2) Self-Audit Checklist (All Gates)
- [x] **Gate 0:** Artifact-first skeleton committed; repo/file/commit links attached in task `githubUrls`.
- [x] **Gate 1:** 7–8 verified active remote leads present (exactly 7).
- [x] **Gate 2:** >=5 leads sourced from Feb 2026 WIH thread.
- [x] **Gate 3:** Primary list TS/Python aligned.
- [x] **Gate 4:** Contact/apply path captured from original HN post for each lead.
- [x] **Gate 5:** Compensation normalized with assumptions documented.
- [x] **Gate 6:** Full per-lead schema complete in CSV.
- [x] **Gate 7:** Decision layer complete: top-3 + outreach drafts + continue/pause recommendation.

## 3) Gate-by-Gate Evidence Table
| Gate | Requirement | Status | Evidence |
|---|---|---|---|
| 0 | Skeleton artifact + links attached | ✅ | Skeleton commits: `6fefec2` (report), `42f6214` (CSV) |
| 1 | 7–8 verified active remote leads | ✅ | `artifacts/lead_shortlist.csv` contains 7 qualified leads |
| 2 | >=5 from Feb 2026 WIH | ✅ | All 7 map to Feb 2026 WIH canonical comment IDs |
| 3 | TS/Python alignment | ✅ | `ts_python_signal` populated for all leads |
| 4 | Contact/apply path | ✅ | `contact_or_apply_path` populated for all leads |
| 5 | Compensation normalization | ✅ | `comp_usd_annual_min/max` + `annualization_method` filled |
| 6 | Full schema | ✅ | All required columns complete including risk + notes |
| 7 | Decision layer | ✅ | Sections 5, 6, and 7 below |

## 4) Final Primary Shortlist (7)
1. **Goody** — Staff/Senior SWE — Remote Americas — TS explicit, Python accepted — $150k–$250k.
2. **FetLife** — Senior DevOps Engineer — Remote — TS in stack context — $115k–$180k.
3. **Greenline** — Founding Engineer (Backend+Data) — Remote US — TypeScript monorepo — $175k–$225k.
4. **Reef Technologies** — Senior Python Backend Engineer — Fully remote — $45–70/hr annualized to $93.6k–$145.6k.
5. **Piq Energy** — Full Stack Software Engineer — US Remote/SF/Athens — TS+Python+AI agents — $150k–$250k.
6. **Wolf Games** — Software Engineer (AI Web Game) — Fully remote US — TS — $45–55/hr annualized to $93.6k–$114.4k.
7. **Wave** — Applied AI Engineer — Remote with country hubs — Python backend + TS frontend stack — up to $222,700.

## 5) Top-3 Prioritized Targets
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

## 6) Outreach Drafts (Top-3)
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

## 7) Recommendation
**Recommendation: CONTINUE**

Execution plan:
1. Submit top-3 immediately (Wave, Piq, Goody).
2. Submit Greenline and Reef as near-parallel alternates.
3. Keep FetLife/Wolf as conditional options depending on role preference (DevOps and contract-to-hire).

## 8) Feasibility Note — Strict 12–15 Feb Slice
Sage feeder evidence (`nrm5CuBN7Q5drmiNF2eQw`, report `ZxiI9jio6LQ2RS_gSMICR`) is persisted in `artifacts/window_scan_2026-02-12_to_2026-02-15.csv`.

In that narrow slice, only Areto had remote + compensation text + Python signal, but compensation was non-numeric and remote was Canada-only. Therefore, the primary 7-lead package uses broader Feb 2026 WIH coverage to meet gate volume and schema requirements while retaining strict-slice transparency.

## 9) Feeder Reconciliation Update (ASAP)
Feeder evidence was reconciled to close adversary gap details:
- Research project: `nrm5CuBN7Q5drmiNF2eQw`
- Report: `ZxiI9jio6LQ2RS_gSMICR`
- Parent thread: https://news.ycombinator.com/item?id=46857488

Exact Areto compensation text is now aligned in strict-window artifact as:
> "Competitive salary + equity, comprehensive benefits, 100% remote"

Confirmed blocker in strict Feb 12–15 slice:
- No numeric compensation ranges for remote TS/Python engineering leads.
- Only qualitative compensation signal appears (Areto), with Canada-only remote constraint.

---
All 8 gates are evidenced in-file and tied to committed artifacts.
