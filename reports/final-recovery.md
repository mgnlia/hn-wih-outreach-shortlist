# Final Recovery — HN WIH Outreach Shortlist (Complete)

Task: `MN-kANIAtC4Vsnl8oOMp9`  
Status: `in_progress`  
Owner: Dev  
Date: 2026-02-13

Source thread (primary): **Ask HN: Who is hiring? (February 2026)**  
https://news.ycombinator.com/item?id=46857488

## 1) Outcome Summary
Finalized a **7-lead** shortlist (required 7–8) of remote/explicit-remote opportunities with compensation published in HN WIH, direct contact/apply paths, TS/Python alignment notes, normalized compensation fields, fit scoring, and risk flags.

Primary data artifact:
- `artifacts/lead_shortlist.csv`

Supplemental scope-check artifact:
- `artifacts/window_scan_2026-02-12_to_2026-02-15.csv`

## 2) Acceptance Checklist (Completed)
- [x] **Gate 0 (checkpoint requirement):** GitHub artifact skeleton committed, with report + checklist, and links attached to task.
- [x] **Gate 1:** 7–8 verified active remote leads.
- [x] **Gate 2:** At least 5 leads from Feb 2026 HN WIH source thread (or explicit fallback evidence).
- [x] **Gate 3:** Primary list is TS/Python aligned.
- [x] **Gate 4:** Contact/apply path captured from original HN post for every lead.
- [x] **Gate 5:** Compensation normalized with assumptions documented.
- [x] **Gate 6:** Full per-lead schema complete in CSV.
- [x] **Gate 7:** Decision layer complete (top-3 targets + outreach drafts + continue/pause recommendation).

## 3) Gate-by-Gate Evidence Table
| Gate | Requirement | Status | Evidence |
|---|---|---|---|
| 0 | Skeleton artifact + links attached to task | ✅ | Commits `6fefec2` and `42f6214`; task githubUrls updated |
| 1 | 7–8 verified active remote leads | ✅ | `artifacts/lead_shortlist.csv` has 7 rows, all remote/explicit-remote |
| 2 | >=5 leads from Feb 2026 WIH thread | ✅ | All 7 leads map to HN comments under thread `46857488` |
| 3 | TS/Python-aligned primary list | ✅ | `ts_python_signal` field completed on all leads |
| 4 | Contact/apply path from original HN post | ✅ | `contact_or_apply_path` filled for all leads |
| 5 | Compensation normalization + assumptions | ✅ | `comp_usd_annual_min/max` and `annualization_method` completed |
| 6 | Full schema completion | ✅ | All required columns populated including risks + notes |
| 7 | Top-3 + outreach drafts + recommendation | ✅ | Sections 5–7 in this report |

## 4) Shortlist (7 Leads)
1. **Goody** — Staff/Senior SWE — Remote (Americas), TS explicit, Python backend accepted, $150k–$250k.
2. **FetLife** — Senior DevOps Engineer — Remote, TS in stack context, $115k–$180k.
3. **Greenline** — Founding Engineer (Backend+Data) — Remote US, TypeScript monorepo, $175k–$225k + equity.
4. **Reef Technologies** — Senior Python Backend Engineer — Fully remote, $45–70/hr annualized to $93.6k–$145.6k.
5. **Piq Energy** — Full Stack SWE — US Remote/SF/Athens, TS+Python+AI agents, $150k–$250k (location-adjusted risk).
6. **Wolf Games** — Software Engineer (AI Web Game) — Fully remote US, TS, $45–55/hr annualized to $93.6k–$114.4k.
7. **Wave** — Applied AI Engineer — Remote with country hubs, Python backend + TS frontend stack, up to $222,700 + equity.

## 5) Top-3 Targets
### #1 Wave — Applied AI Engineer
- Strongest direct AI-agent relevance.
- Python-heavy backend fit + large-scale agent interaction ownership.
- High compensation ceiling.

### #2 Piq Energy — Full Stack SWE
- Explicit TS + Python + AI agent workflow alignment.
- End-to-end ownership matches full-stack AI profile.
- Strong base comp range.

### #3 Goody — Staff/Senior SWE
- Clear TS product engineering fit with Python backend flexibility.
- Multiple openings and direct CTO contact path.
- Competitive compensation band.

## 6) Outreach Drafts
### Draft A — Wave
Subject: Applied AI Engineer (HN Feb WIH) — Python + agent systems

Hi Wave team — I’m reaching out regarding your HN posting for the Applied AI Engineer role. I build and ship production AI systems with a strong Python backend focus, including agent orchestration/evaluation workflows and reliability hardening in user-facing products.

Your focus on autonomous voice/digital agents at scale is exactly the domain I’m targeting. I’ve applied via the careers link and wanted to add a direct note that I came from the HN thread.

Best,  
[Name]

### Draft B — Piq Energy
Subject: Full Stack SWE (HN) — TypeScript/Python + agent workflows

Hi Piq Energy team — I saw your HN WIH post and am very interested in the Full Stack SWE role. I’m a TS/Python-focused engineer and have built end-to-end systems spanning frontend product surfaces, backend APIs, pipelines, and LLM-agent workflows.

Your stack and mission are a strong fit; I’d be glad to discuss where I could contribute fastest.

Best,  
[Name]

### Draft C — Goody
Subject: HN WIH — Staff/Senior SWE interest (TypeScript + Python backend)

Hi Mark — I’m reaching out from your Feb HN WIH post for Goody engineering roles. I’m a full-stack engineer with strong TypeScript delivery and Python backend depth, and I’m excited by high-ownership startup execution.

I’d be happy to share concise examples of recent TS/Python systems and results.

Best,  
[Name]

## 7) Recommendation
**Recommendation: CONTINUE**

Execution order:
1. Submit top-3 immediately (Wave, Piq, Goody).
2. Submit Greenline and Reef next as strong alternates.
3. Treat FetLife/Wolf as conditional options depending on preference for DevOps and contract-to-hire models.

## 8) Exclusions / Constraints
Not in primary due to explicit constraints from feeder evidence:
- Onsite-only: Duolingo, Faraday, Pepr AI.
- Hybrid-only: Bidaya AI.
- Weaker TS/Python signal for primary objective: Category Labs, Runable, EnigmoFi.

## 9) Supplemental Strict-Window Check (Feb 12–15)
Using feeder evidence from Sage (`G4-2zuBSSMF9xvXbk3ZhG`, research project `nrm5CuBN7Q5drmiNF2eQw`, report `ZxiI9jio6LQ2RS_gSMICR`), a strict scan for Feb 12–15 was persisted to `artifacts/window_scan_2026-02-12_to_2026-02-15.csv`.

Result summary:
- 8 canonical candidates in-window.
- Only **Areto Labs** matched remote + comp-published + Python signal, but compensation was qualitative (non-numeric) and remote was Canada-only.
- No in-window lead satisfied the full ideal filter of remote + published numeric compensation + strong TS/Python signal at the target count.

Implication:
- The primary 7-lead deliverable remains based on broader Feb 2026 WIH coverage to satisfy acceptance volume and schema-completeness requirements, while preserving strict-window evidence transparently.

---
This report and CSV together satisfy all acceptance gates while keeping task status in `in_progress` pending Henry confirmation.
