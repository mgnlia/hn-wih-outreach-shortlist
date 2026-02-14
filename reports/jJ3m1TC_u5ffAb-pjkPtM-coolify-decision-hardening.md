# Coolify Debian 13 Triage — Decision Hardening Dossier (`jJ3m1TC_u5ffAb-pjkPtM`)

Date: 2026-02-14

## 1) Canonical issue + competing PR/claim map

### Canonical issue (source of truth)
- Bounty issue: https://github.com/coollabsio/coolify/issues/8154
  - Labels include **$6.9k** and **💎 Bounty**.
  - Requirement in issue body: *"Before you start implementing this feature for the bounty you must share your implementation plan below in the comments."*

### Root bug context
- Debian 13 install failure context: https://github.com/coollabsio/coolify/issues/6405
  - Shows Docker repo failure path for Debian 13 (`trixie`) and prerequisite installation breakage.

### Competing implementation evidence
- Closed competing PR linked to bounty path:
  - https://github.com/coollabsio/coolify/pull/8206
  - Contains `/claim #8154` and Debian13 fallback + Alpine prerequisite changes.
- Additional competition map artifact:
  - `artifacts/jJ3m1TC_u5ffAb-pjkPtM_coolify_competing_pr_map.csv`
  - Includes high-confidence pending claims and medium-confidence overlapping claim pages.

## 2) Maintainer-validated acceptance checklist
Checklist is constrained to maintainer-stated requirement in #8154 plus reproducible success criteria implied by #6405 failure mode and existing claim flow.

- [ ] **Pre-implementation plan posted in #8154 comments** (explicitly required by maintainer in issue body).
- [ ] Debian 13 server passes additional-server validation in Coolify.
- [ ] Prerequisite installer no longer fails on Debian 13 Docker repo path.
- [ ] Debian codename handling includes safe fallback behavior for `trixie` when native Docker repo is unavailable.
- [ ] Alpine prerequisites handling does not regress existing server onboarding flows.
- [ ] Evidence includes reproducible install/validation logs.
- [ ] Bounty syntax and claim metadata are correct (e.g., `/claim #8154`) in PR/issue flow.

## 3) Claimability assessment

### Is claim still open?
- Issue #8154 remains open and labeled bounty.
- However, claimability is **contested** rather than cleanly open due to visible pending claims and at least one closed competing PR with claim syntax.

### Claimability verdict
- **Formally claimable:** Yes (issue open).
- **Practically claimable with favorable odds:** Weak under current saturation.

## 4) Win probability model

Assumptions:
- Competitive implementation effort: **8–14h**
- Contest state: multiple overlapping claim attempts already visible
- Merge-order + maintainer preference uncertainty: high

Estimated **P(win)** now: **4–10%** (tightened down from prior 5–12% after adding explicit closed PR evidence).

## 5) ROI estimate

- Nominal bounty: **$6,900**
- Gross EV = `6900 * P(win)` = **$276–$690**
- EV/hour over 8–14h = **~$20–$86/h** before iteration overhead and payout-process friction.

Interpretation: risk-adjusted expected return is below target compared to less-contested opportunities.

## 6) GO/PARK recommendation

## **Recommendation: PARK (NO-GO this cycle)**

Rationale:
1. High claim/PR saturation on identical scope.
2. Elevated duplicate-work risk.
3. Reduced risk-adjusted EV despite attractive headline bounty.

## 7) Re-open triggers (monitor-only)
- Pending claim(s) rejected/withdrawn.
- Maintainer requests additional independent implementation due unresolved gap.
- Scope split creates unclaimed sub-problem with clear acceptance boundary.

Until one trigger occurs, continue **PARK** and allocate effort to less-contested TS/Python-aligned lanes.
