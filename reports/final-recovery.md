# Final Recovery — HN WIH Outreach Shortlist (Final QA Package, 9 Gates)

Task: `MN-kANIAtC4Vsnl8oOMp9`  
Status: `in_progress`  
Owner: Dev  
Date: 2026-02-14

Primary source thread: **Ask HN: Who is hiring? (February 2026)**  
https://news.ycombinator.com/item?id=46857488

## 1) Outcome Summary
Delivered a **7-lead primary shortlist** (required 7–8) of remote/explicit-remote Feb 2026 WIH opportunities with:
- active verification signals,
- TS/Python fit enforcement,
- contact/apply paths,
- normalized compensation fields in USD annualized form,
- prioritization and outreach drafts.

Primary artifacts:
- `artifacts/lead_shortlist.csv`
- `reports/final-recovery.md`

Supplemental feasibility artifact:
- `artifacts/window_scan_2026-02-12_to_2026-02-15.csv`

## 2) Gate Definitions (Final Cycle: 9 Gates)
- **Gate 0:** Artifact links present (repo + files + commit links in task `githubUrls`).
- **Gate 1:** 7–8 active verified leads (no placeholders/TBD rows).
- **Gate 2:** Recency target and fallback evidence explicit.
- **Gate 3:** Feb 2026 WIH provenance (>=5 leads from thread).
- **Gate 4:** TS/Python fit enforcement across retained leads.
- **Gate 5:** Contact/apply paths captured for each lead.
- **Gate 6:** Compensation normalization to USD annual fields with method notes.
- **Gate 7:** Decision layer complete (Top-3 + outreach drafts + continue/pause recommendation).
- **Gate 8:** Self-audit table mapping each gate to exact evidence location.

## 3) Self-Audit Checklist
- [x] Gate 0 — artifact links present
- [x] Gate 1 — 7 active verified leads
- [x] Gate 2 — recency target + fallback explicit
- [x] Gate 3 — WIH provenance satisfied
- [x] Gate 4 — TS/Python enforcement satisfied
- [x] Gate 5 — contact/apply paths complete
- [x] Gate 6 — USD normalization complete
- [x] Gate 7 — Top-3 + drafts + recommendation complete
- [x] Gate 8 — gate-to-evidence table present

## 4) Self-Audit Table — Gate → Evidence
| Gate | Requirement | Status | Evidence location |
|---|---|---|---|
| 0 | Repo/file/commit links in task | ✅ | Task `githubUrls` includes repo + blob links + latest commits |
| 1 | 7–8 active verified leads; no placeholder rows | ✅ | `artifacts/lead_shortlist.csv` has exactly 7 rows (`HN-WIH-2026-001..007`) and no `TBD` entries |
| 2 | Recency target + fallback evidence | ✅ | Section 5 below + `posting_date_utc` in CSV + strict-window fallback artifact |
| 3 | >=5 leads from Feb WIH thread | ✅ | `hn_canonical_url` populated for all 7 leads (all from Feb WIH thread) |
| 4 | TS/Python fit enforcement | ✅ | `ts_python_signal` complete for all 7 leads; Section 6 matrix |
| 5 | Contact/apply per lead | ✅ | `contact_or_apply_path` complete for all 7 leads |
| 6 | USD normalized compensation + method | ✅ | `comp_usd_annual_min/max` + `annualization_method` complete (with max-only note where applicable) |
| 7 | Top-3 + drafts + recommendation | ✅ | Sections 8, 9, 10 |
| 8 | Self-audit gate mapping in report | ✅ | Section 4 (this table) |

## 5) Recency Target and Fallback Evidence
### Target window (strict): 2026-02-12 to 2026-02-15
Evidence file: `artifacts/window_scan_2026-02-12_to_2026-02-15.csv`
- Confirmed strict-window blocker: numeric compensation ranges for remote TS/Python engineering roles were not available in this narrow slice.
- Best strict-window partial: Areto (qualitative compensation only; Canada-only remote constraint).

### Fallback window (executed): broader Feb 2026 WIH
To satisfy lead-count and schema gates, the primary shortlist used broader February WIH coverage with explicit transparency.

Recency values in final shortlist (`posting_date_utc`):
- 2026-02-02: HN-WIH-2026-001, 002, 003, 005
- 2026-02-03: HN-WIH-2026-004, 006
- 2026-02-11: HN-WIH-2026-007

## 6) TS/Python Fit Enforcement Matrix
- HN-WIH-2026-001 (Goody): **TypeScript explicit; Python accepted backend**
- HN-WIH-2026-002 (FetLife): **TypeScript present in stack context**
- HN-WIH-2026-003 (Greenline): **TypeScript explicit**
- HN-WIH-2026-004 (Reef): **Python explicit**
- HN-WIH-2026-005 (Piq): **TypeScript + Python + AI agents explicit**
- HN-WIH-2026-006 (Wolf): **TypeScript explicit**
- HN-WIH-2026-007 (Wave): **Python backend explicit; TypeScript frontend in stack**

## 7) Final Primary Shortlist (7 Active Verified Leads)
1. **Goody** — Staff/Senior SWE — Remote Americas — TS explicit, Python accepted — $150k–$250k.
2. **FetLife** — Senior DevOps Engineer — Remote — TS in stack context — $115k–$180k.
3. **Greenline** — Founding Engineer (Backend+Data) — Remote US — TypeScript monorepo — $175k–$225k.
4. **Reef Technologies** — Senior Python Backend Engineer — Fully remote — $45–70/hr annualized to $93.6k–$145.6k.
5. **Piq Energy** — Full Stack Software Engineer — US Remote/SF/Athens — TS+Python+AI agents — $150k–$250k.
6. **Wolf Games** — Software Engineer (AI Web Game) — Fully remote US — TS — $45–55/hr annualized to $93.6k–$114.4k.
7. **Wave** — Applied AI Engineer — Remote hubs — Python backend + TS frontend — up to $222,700.

## 8) Top-3 Prioritized Targets
### #1 Wave — Applied AI Engineer
- Highest direct fit for Python + production AI-agent systems.
- Large-scale real-world deployment context.
- Strong compensation ceiling.

### #2 Piq Energy — Full Stack Software Engineer
- Explicit TS/Python/AI-agent stack.
- End-to-end product ownership scope.
- Strong pay band.

### #3 Goody — Staff/Senior Software Engineer
- Strong TS execution fit with Python flexibility.
- Multiple role lanes + direct contact path.
- Attractive compensation range.

## 9) Outreach Drafts (Top-3)
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

## 10) Recommendation
**Recommendation: CONTINUE**

Execution sequence:
1. Apply immediately to Wave, Piq, Goody.
2. Follow with Greenline + Reef as near-parallel alternates.
3. Keep FetLife/Wolf as conditional based on preference (infra/game contract track).

## 11) Evidence Gap (Explicitly Labeled)
- **Data gap:** strict 12–15 Feb slice does not provide numeric compensation ranges for remote TS/Python engineering leads.
- **Consequence:** strict-window-only package would fail gate volume + normalization strictness.
- **Mitigation:** retain strict-window artifact for transparency and use broader Feb WIH fallback for final compliant package.

---
Final package is fully populated (no placeholders), with all 9 gates evidenced and cross-referenced.
Status intentionally remains `in_progress` until explicit approval to move `review`.
