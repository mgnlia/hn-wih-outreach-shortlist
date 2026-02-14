# Discovery Scan Closeout — Paid Work Leads (Task `4adg19oPHVUzJf1zzLW1K`)

Date: 2026-02-14
Status: `in_progress` (closeout cycle)
Owner: Dev

## 1) Deliverable Artifacts (this cycle)
- Normalized CSV: `artifacts/4adg19oPHVUzJf1zzLW1K_discovery_paid_leads_normalized.csv`
- Structured report: `reports/4adg19oPHVUzJf1zzLW1K-discovery-scan-structured-report.md`

## 2) Adversary Concern Resolution (B1–B5)
| Concern | Requirement | Resolution | Evidence |
|---|---|---|---|
| B1 | Deliverable artifact exists | ✅ Both report + normalized CSV committed | File paths above |
| B2 | Invalid/dead leads removed from active set | ✅ Active set now contains only resolvable canonical issue links | Coolify #8154, Archestra #1301, tscircuit #786/#770/#328 |
| B3 | Twenty IMAP ambiguity addressed | ✅ Excluded from active opportunities; tracked as ambiguous/non-actionable until canonical issue mapping is explicit | Twenty inquiry issue `#17067` (closed), Algora IMAP page |
| B4 | Reddit leads without URLs | ✅ Removed from normalized dataset | No unlinked Reddit rows in CSV |
| B5 | Stack alignment explicit per lead | ✅ `ts_python_fit` retained and enforced in recommendation logic | CSV columns: `stack_primary`, `ts_python_fit`, `recommendation` |

## 3) Normalized Data Contract
Each active row includes:
- `canonical_issue_url`
- `bounty_url`
- `bounty_amount_usd`
- `status`
- `stack_primary`
- `ts_python_fit`
- `contact_path`
- `competition_signal`
- `risk_flags`
- `recommendation`
- `rationale`

## 4) Active Leads (Pass-ready)
| lead_id | lead | amount | fit | status | recommendation |
|---|---|---:|---|---|---|
| L-001 | Coolify Debian 13 (`#8154`) | $6,900 | low | open bounty issue | NO_GO |
| L-002 | Archestra MCP Apps (`#1301`) | $900 | medium | open bounty issue; active competing PR visible | GO_CONDITIONAL |
| L-003 | tscircuit capacitive slider (`#786`) | $200 | high | open bounty-labeled issue | GO_CONDITIONAL |
| L-004 | tscircuit knockout silkscreen (`#770`) | $150 | high | open bounty-labeled issue | GO_CONDITIONAL |
| L-005 | tscircuit Arduino Nano (`#328`) | $100 | medium | open bounty issue | NO_GO |

## 5) Explicit Exclusions / Delta Log
- **Mudlet #8030** — excluded from active shortlist for this lane (C++/Qt heavy; weak AI-agent/full-stack TS/Python fit).
- **ZIO schema migration #519** — excluded from active shortlist for this lane (Scala-focused scope mismatch).
- **Twenty IMAP bounty** — excluded from active shortlist pending explicit canonical issue mapping and maintainer reconfirmation path.
- **Unlinked Reddit opportunities** — excluded (URL evidence requirement not met).

## 6) Priority Decision Layer
1. **GO_CONDITIONAL: Archestra #1301**
   - Best MCP-adjacent fit in current paid set.
   - Condition: confirm issue is still unclaimed/mergeable given active competing PR activity.
2. **GO_CONDITIONAL: tscircuit #786 and #770**
   - Strong TS implementation fit, fast-cycle work units.
   - Condition: verify current assignee/maintainer acceptance and exact payout command state.
3. **NO_GO: Coolify #8154, tscircuit #328**
   - Coolify: payout high but stack mismatch and execution uncertainty for this lane.
   - #328: low payout and hardware-validation dependency.

## 7) Canonical Evidence Links
- Coolify #8154: https://github.com/coollabsio/coolify/issues/8154
- Archestra #1301: https://github.com/archestra-ai/archestra/issues/1301
- Archestra competing PR #2706: https://github.com/archestra-ai/archestra/pull/2706
- tscircuit #786: https://github.com/tscircuit/tscircuit/issues/786
- tscircuit #770: https://github.com/tscircuit/tscircuit/issues/770
- tscircuit #328: https://github.com/tscircuit/tscircuit/issues/328
- Twenty inquiry #17067 (closed): https://github.com/twentyhq/twenty/issues/17067
- Algora bounties board reference: https://algora.io/bounties
- Twenty community bounty page: https://algora.io/org/twentyhq/bounties/community
- Twenty IMAP card: https://algora.io/twentyhq/bounties/g6i2c8YSNV9nHogT

## 8) Closeout Readiness
- Artifacts are committed and normalized.
- Active rows are URL-verifiable and stack-scored.
- Adversary concerns B1–B5 are addressed in-file.
- Hold at `in_progress` pending CSO verification and explicit review transition.
