# Discovery Normalization Resubmission — Paid Work Leads (Task `4adg19oPHVUzJf1zzLW1K`)

Date: 2026-02-14

## Deliverable artifacts
- Normalized lead table (per-lead schema):
  - `artifacts/4adg19oPHVUzJf1zzLW1K_discovery_paid_leads_normalized.csv`
- This structured report:
  - `reports/4adg19oPHVUzJf1zzLW1K-discovery-scan-structured-report.md`

## What changed vs failed submission
This resubmission resolves B1–B5:

1. **B1 (No deliverable artifact)** → Added committed report + normalized CSV with required fields:
   - URL (`canonical_issue_url` + `bounty_url`)
   - bounty amount (`bounty_amount_usd`)
   - status (`status`)
   - stack (`stack_primary` + `ts_python_fit`)
   - contact path (`contact_path`)
   - risk flags (`risk_flags`)

2. **B2 (Invalid issues)** → Removed invalid/dead leads from active table:
   - Mudlet #8030 (no payout-confidence for our scope, stack mismatch)
   - zio-schema #519 (closed/rewarded)

3. **B3 (Twenty IMAP likely dead)** → Marked as unavailable and excluded from active targets.
   - Status inquiry issue is closed as Done:
     - https://github.com/twentyhq/twenty/issues/17067
   - Algora org page shows IMAP bounty in completed set:
     - https://algora.io/org/twentyhq/bounties/community

4. **B4 (Reddit leads missing URLs)** → Removed unlinked Reddit claims from normalized table.

5. **B5 (Stack alignment gap)** → Rebalanced toward TS-fit opportunities (Archestra + tscircuit set), and explicitly labeled out-of-stack opportunities as low fit.

## Active normalized leads (decision snapshot)
| lead_id | lead | amount | stack fit | status | recommendation |
|---|---|---:|---|---|---|
| L-001 | Coolify Debian 13 | $6,900 | Low (PHP) | Open, high claim activity | NO_GO |
| L-002 | Archestra MCP Apps #1301 | $900 | Medium | Open bounty | GO |
| L-003 | tscircuit #786 | $200 | High (TS) | Open bounty label | GO_CONDITIONAL |
| L-004 | tscircuit #770 | $150 | High (TS) | Open bounty label | GO_CONDITIONAL |
| L-005 | tscircuit #328 | $100 | Medium (TS) | Open bounty | NO_GO |

## Excluded/invalid leads log
- **Mudlet #8030** — excluded from this lane (poor stack fit + low relevance for AI-agent/full-stack scope).
- **zio-schema #519** — excluded; closed and rewarded.
- **Twenty IMAP** — excluded as high-risk/unavailable until maintainer reconfirms new payable scope.
- **Reddit AI CCTV / chatbot contract references** — excluded due to missing verifiable URLs.

## Stack alignment summary
- In active table, **3/5 leads are TypeScript-first** (tscircuit set), 1 is medium-fit MCP/UI (Archestra), 1 is high-$ but out-of-stack (Coolify).
- Out-of-stack entries are retained only when payout/market signal is large enough to evaluate opportunity cost explicitly.

## Priority recommendation
1. **GO: Archestra #1301** (best near-term TS/MCP-adjacent paid target).
2. **Conditional TS backups: tscircuit #786, #770** (small-dollar, fast-cycle candidates).
3. **Deprioritize/No-go: Coolify for this lane due to stack mismatch + claim saturation; Twenty IMAP unavailable without reconfirmation.**

## Canonical source links
- Archestra #1301: https://github.com/archestra-ai/archestra/issues/1301
- Coolify #8154: https://github.com/coollabsio/coolify/issues/8154
- Twenty status inquiry #17067: https://github.com/twentyhq/twenty/issues/17067
- Twenty completed bounties page: https://algora.io/org/twentyhq/bounties/community
- tscircuit #786: https://github.com/tscircuit/tscircuit/issues/786
- tscircuit #770: https://github.com/tscircuit/tscircuit/issues/770
- tscircuit #328: https://github.com/tscircuit/tscircuit/issues/328
- Algora board reference: https://algora.io/bounties
