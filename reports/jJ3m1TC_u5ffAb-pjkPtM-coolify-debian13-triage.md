# Triage — Coolify Debian 13 support bounty (`jJ3m1TC_u5ffAb-pjkPtM`)

Date: 2026-02-14  
Decision target: **Go / No-Go within current cycle**

## 1) Canonical links + maintainer confirmation path

### Canonical bounty/issue links
- GitHub issue (canonical): https://github.com/coollabsio/coolify/issues/8154
- Algora bounty board (shows Coolify #8154 at $6,900): https://algora.io/bounties
- Algora claim page linked to #8154 (status evidence): https://algora.io/claims/6bdZBHqmWqedLz2A
- Related root bug context (Debian 13 Docker repo failure): https://github.com/coollabsio/coolify/issues/6405

### Maintainer confirmation / claim path
From issue/bounty instructions and linked bounty flow:
1. Comment on issue with implementation plan using: **`/attempt #8154`**
2. Open PR with claim marker in PR body: **`/claim #8154`**
3. Payment is processed post-reward (Algora flow; typically 2–5 days after reward approval).

**Important confirmation needed before coding:**
- Whether bounty is still available for new attempts while an existing submission is pending.
- Whether payout is currently **$6,900** vs pooled **$13,800** (Algora claim page shows total prize pool $13,800 from two sponsors).

## 2) Acceptance criteria extraction (testable checklist)

Issue #8154 requirement excerpt: make Coolify validate additional servers running Debian 13 during connect/validate flow.

### Testable checklist
- [ ] Debian 13 host is recognized as supported OS during additional-server validation.
- [ ] Docker install prerequisite step does not fail when Debian codename/repo mapping is unresolved.
- [ ] Fallback strategy for Docker APT repo is implemented (e.g., codename-aware with fallback when trixie repo is unavailable).
- [ ] "Validate & Install" succeeds end-to-end on Debian 13.
- [ ] Regression safety: Debian 12/Ubuntu existing flows still pass.
- [ ] Unit/integration test added for fallback logic.
- [ ] Lint/style checks pass and PR includes `/claim #8154`.

## 3) Claimability + competition assessment

## Current signals
- Issue #8154 is open and labeled bounty.
- Algora claim page shows: **Status: Pending**, **Submitted: 2026-02-10**, with a named contributor and demo/test notes.

## Competition risk
- **High** near-term competition risk due pending submission already present.
- If maintainer accepts pending submission first, expected value for a new parallel implementation drops sharply.
- If maintainer requests revisions / no merge, there may still be entry opportunity for a cleaner/faster PR.

## Claimability verdict
- **Claimable only conditionally** pending maintainer clarification in-thread.

## 4) Effort/risk estimate + recommendation

## Estimated implementation effort (if greenlit)
- Repo familiarization + reproduce on Debian 13: **1.5–3h**
- Implement detection/fallback logic: **2–4h**
- Add tests + regression checks: **2–4h**
- PR polish + maintainer iteration buffer: **1–3h**

**Total:** ~**6.5–14h** (single engineer), with schedule risk driven by maintainer feedback and live competitor submission.

## Technical risks
- Docker upstream repo/codename behavior may shift; fallback must avoid brittle hardcoding.
- Need to avoid regressions for existing distro detection/install logic.
- Potential duplicate work if pending claimant already converged on maintainers’ preferred patch.

## Recommendation
**GO (conditional gate)**
- Proceed **only if** maintainer confirms in #8154 comments that additional attempts are welcome despite pending submission.
- If no confirmation within SLA window (e.g., 6–12 hours), switch to **NO-GO for this cycle** and reallocate to open bounties with no pending claimant.

## Fast execution plan for Dev (if GO confirmed)
1. Post `/attempt #8154` with concise implementation plan + test matrix.
2. Reproduce Debian 13 failure path from #6405.
3. Implement codename-aware Docker repo fallback with safe default path.
4. Add focused test(s) for fallback behavior.
5. Open PR with `/claim #8154` and attach reproduce/proof logs.

---

## Evidence quality notes
- GitHub issue and related bug are canonical and high-confidence.
- Algora claim page indicates active pending submission and potential pooled sponsorship.
- Payout amount ambiguity ($6,900 vs pooled $13,800) should be resolved with maintainer/Algora in-thread before committing engineering hours.
