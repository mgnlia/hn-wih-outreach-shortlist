# Coolify Debian 13 Bounty — Initial Evidence Commit (T+60 package)

Task: `jJ3m1TC_u5ffAb-pjkPtM`  
Timestamp: 2026-02-14

## Canonical evidence
- Primary issue: https://github.com/coollabsio/coolify/issues/8154
- Related failure context: https://github.com/coollabsio/coolify/issues/6405
- Algora board listing (shows open Coolify #8154 at $6,900): https://algora.io/bounties
- Algora claim page for this issue: https://algora.io/claims/6bdZBHqmWqedLz2A

## Extracted acceptance checklist (testable)
- [ ] Additional server validation accepts Debian 13 hosts in Coolify server onboarding flow.
- [ ] Prerequisite installation no longer fails for Debian 13 when Docker Debian repo/codename path is unavailable.
- [ ] Implement codename-aware Docker apt fallback (safe fallback if trixie unavailable).
- [ ] “Validate & Install” completes end-to-end on Debian 13 host.
- [ ] Regression checks pass for Debian 12 and Ubuntu flows.
- [ ] Add focused automated test for fallback logic.
- [ ] PR includes `/claim #8154` marker and reproducible test/log evidence.

## Competition map (initial)
| lane | source | status | date signal | competition risk | confidence |
|---|---|---|---|---|---|
| Direct issue bounty | https://github.com/coollabsio/coolify/issues/8154 | Open issue, bounty labeled | opened 2026-02-05 | Medium | High |
| Existing claimant submission | https://algora.io/claims/6bdZBHqmWqedLz2A | **Pending** submission listed | submitted 2026-02-10 | **High** | High |
| Historical root bug | https://github.com/coollabsio/coolify/issues/6405 | Open bug context and repro logs | opened 2025-08-20 | Low (context) | High |

## Maintainer confirmation path to de-risk duplicate work
1. Post `/attempt #8154` with precise implementation plan.
2. Ask maintainer to confirm whether additional concurrent attempts are welcome despite pending claim.
3. If confirmed, proceed with implementation and PR including `/claim #8154`.

## Interim call
- **Interim status: CONDITIONAL GO**
- Blocker: unresolved exclusivity/priority vs existing pending claimant.
- Next step: get maintainer clarification in-thread before committing full engineering cycle.
