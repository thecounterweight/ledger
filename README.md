# The Counterweight — Public Ledger

Every contribution received and every rupee spent, recorded permanently.

## How to verify

1. Clone this repo
2. Check `git log --show-signature` — every entry is GPG-signed
3. The git hash chain guarantees tamper-evidence — alter one entry and all subsequent hashes break
4. External archives at [archive.org](https://web.archive.org/web/*/github.com/thecounterweight/ledger) and [Software Heritage](https://archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/thecounterweight/ledger)

## Structure

```
contributions/
  YYYY-MM-DD_name_amount.md    # Signed promissory note record
spending/
  YYYY-MM-DD_purpose_amount.md # What was spent and why
BALANCE.md                     # Running total
```

## Rules

- Every entry is a separate commit, GPG-signed by the founder
- No entry is ever deleted — corrections are new commits that reference the original
- Balance is updated with every contribution or expenditure
- Anyone can audit the full history at any time

## Current status

No contributions received yet. The ledger activates with the first contribution.

## Related

- [Funding Model](https://github.com/thecounterweight/platform/blob/main/docs/funding-model.md) — how contributions work
- [Contribution Agreement Template](https://github.com/thecounterweight/platform/blob/main/docs/contribution-agreement-template.md) — the agreement contributors sign
