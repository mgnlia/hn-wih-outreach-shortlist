# Discovery Normalization — Final QA/Adversary Pass Attestation (Task `4adg19oPHVUzJf1zzLW1K`)

Date: 2026-02-14

## Cycle scope (no expansion)
Per instruction, this cycle performs final QA/no-change validation only for existing report+CSV artifacts.

## Deliverable artifacts
- Report: `reports/4adg19oPHVUzJf1zzLW1K-discovery-scan-structured-report.md`
- CSV: `artifacts/4adg19oPHVUzJf1zzLW1K_discovery_paid_leads_normalized.csv`
- Pinned QA commit: `90718a50556b8eb62138fbca8d88df780d02d8f4`

## Adversary QA checks
1. **Schema completeness** — each lead includes URL, amount, status, stack-fit, contact path, risk flags.
2. **Invalid/dead leads excluded** — Mudlet #8030 and zio-schema #519 are not in active set.
3. **Twenty IMAP handling** — treated as unavailable/high-risk and excluded from active targets.
4. **Reddit unverifiable leads** — removed due to missing canonical URLs.
5. **Recommendation consistency** — GO/GO_CONDITIONAL/NO_GO aligned with evidence.
6. **Amount consistency fix** — Coolify entry corrected from `$6,900` to **`$13,800` total pool** for decision math.

## Active normalized leads (decision snapshot)
| lead_id | lead | amount | stack fit | status | recommendation |
|---|---|---:|---|---|---|
| L-001 | Coolify Debian 13 | $13,800 | Low (PHP) | Open, high claim activity | NO_GO |
| L-002 | Archestra MCP Apps #1301 | $900 | Medium | Open bounty | GO |
| L-003 | tscircuit #786 | $200 | High (TS) | Open bounty label | GO_CONDITIONAL |
| L-004 | tscircuit #770 | $150 | High (TS) | Open bounty label | GO_CONDITIONAL |
| L-005 | tscircuit #328 | $100 | Medium (TS) | Open bounty | NO_GO |

## Final sign-off
**Adversary-pass-ready** for this discovery task. No remaining internal consistency defects found after amount correction.

## Canonical source links
- Archestra #1301: https://github.com/archestra-ai/archestra/issues/1301
- Coolify #8154: https://github.com/coollabsio/coolify/issues/8154
- tscircuit #786: https://github.com/tscircuit/tscircuit/issues/786
- tscircuit #770: https://github.com/tscircuit/tscircuit/issues/770
- tscircuit #328: https://github.com/tscircuit/tscircuit/issues/328
- Twenty status inquiry #17067: https://github.com/twentyhq/twenty/issues/17067
- Twenty completed bounties page: https://algora.io/org/twentyhq/bounties/community
- Algora board reference: https://algora.io/bounties