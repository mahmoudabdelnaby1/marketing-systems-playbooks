# Partner and Referral Channel Economics

Use this worksheet alongside the order-level unit economics model when affiliates, creators, referrers, or other partners receive a reward tied to an order. It helps expose the actual partner cost; it does not set a recommended commission rate or predict channel performance.

## Record the commercial terms

| Input | Record |
|---|---|
| Partner/program and market | Name the actual program and applicable market |
| Eligible conversion event | E.g. placed, approved, delivered, or retained order; quote the agreement |
| Commission basis | Percentage, fixed amount, tier, or other contract term |
| Payout trigger and timing | Include validation, cancellation, refund, and reversal terms |
| Customer incentive | Discount or other reward funded by the merchant |
| Additional program costs | Platform, tracking, management, creative, or payment costs |
| Attribution rule | Source, window, precedence, and treatment of overlapping channels |
| Evidence | Contract or approved terms, source, owner, and review date |

## Calculate with reconciled orders

For the same period and order cohort, record:

`net_partner_payouts = approved payouts − contractually reversed payouts`

`partner_cost_per_eligible_order = (net_partner_payouts + merchant-funded incentives + allocated program costs) / eligible orders`

`contribution_after_partner_cost = contribution_before_partner_cost − partner_cost_per_eligible_order`

Keep placed, approved, delivered, and retained orders distinct. Use the contract's actual payout trigger, and do not assume a cancellation or return reverses a commission unless the terms say so. Reconcile partner reports to order IDs and settled amounts before treating the result as realized cost.

## Review before using the result

- Check whether the existing `ad_cost_per_order` already includes partner payouts; avoid counting the same cost twice.
- Separate attributed orders from incremental orders. Attribution alone does not establish that the partner caused the purchase.
- Check duplicate, self-referral, coupon leakage, and invalid-order rules against the actual program terms; do not invent fraud thresholds.
- Keep any disclosure, tax, or consumer-law question specific to the market and current official guidance; refer legal interpretation to qualified counsel.
- Label incomplete periods, unsettled payouts, and assumptions. Do not call a scenario a forecast or case result.
