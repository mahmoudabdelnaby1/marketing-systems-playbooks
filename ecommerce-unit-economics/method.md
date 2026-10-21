# Metric definitions and calculation sequence

Use a consistent cohort and period. Record whether revenue includes tax and whether returns/refunds are already excluded.

## Core calculations

- **Platform-reported ROAS** = platform-attributed revenue ÷ ad spend. Attribution windows and reporting rules differ by platform.
- **Delivered revenue** = revenue associated with delivered orders after the chosen refund/return treatment. Define this treatment explicitly.
- **Delivered-revenue-to-ad-spend ratio** = delivered revenue ÷ ad spend. This is a descriptive ratio, not profit and not automatically comparable to platform ROAS.
- **Contribution before advertising** = recognized revenue − COGS − fulfillment − payment fees − other variable costs included in the model.
- **Contribution after advertising** = contribution before advertising − ad spend.

## Do not mix these items

- Do not apply a single delivery-success percentage to revenue if order values, payment methods, refunds, or product costs vary materially; calculate by segment when the data permits.
- Do not subtract VAT/tax unless the revenue input and accounting treatment require it. Use the business’s actual tax handling.
- Do not subtract an RTO cost twice. Identify which courier, packaging, and handling charges are included in fulfillment costs.
- Do not call contribution “net profit” unless fixed costs, payroll, overhead, financing, and all other relevant costs are included.
- Do not compare platform ROAS and delivered-revenue ratio without stating attribution window, order cohort, and date range.

## Reconciliation

Record source report, export date, timezone, attribution window, and filters. Investigate discrepancies before using the model for decisions.