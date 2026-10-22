# E-commerce Funnel Diagnostic

A store-specific workflow for finding where customer journeys lose progress and separating observed friction from assumptions. It complements `ecommerce-unit-economics` (order contribution and break-even calculations) and `arabic-rtl-cro-auditor` (Arabic and mixed-language usability review).

## Use it when

Traffic, leads, or orders change and the team needs to diagnose the path from source through landing page, product consideration, cart, checkout, and fulfilled order before choosing a change.

## Included

- [`templates/funnel-evidence-log.csv`](templates/funnel-evidence-log.csv): stage counts, definitions, and source register.
- [`templates/diagnostic-decision-record.md`](templates/diagnostic-decision-record.md): hypothesis, test, guardrails, and decision record.

## Workflow

1. State what moved, when, for which segment and source. Separate platform-attributed results from store orders and delivered outcomes.
2. Validate event definitions, counts, currency, deduplication, consent, checkout transitions, and order reconciliation.
3. Map comparable populations through landing page, product view, add to cart, checkout, payment attempt, order, and later fulfillment outcomes where available.
4. Segment by device, source, landing page, product, geography, or payment option only when definitions are consistent and samples support comparison; mark small samples inconclusive.
5. Reproduce the journey on mobile and desktop. Check load, price/shipping clarity, stock, form errors, payment failures, trust information, and support access.
6. Separate observed defects from hypotheses. Choose one focused change with a mechanism, owner, guardrails, and success metric.
7. Test where feasible. Otherwise document the comparison and confounding factors; do not claim causality from a simple before/after.
8. Keep, revise, or revert based on agreed evidence and record the decision and limitations.

## Boundaries

This diagnostic sets no universal conversion thresholds and makes no market-wide claim. Use actual account and store evidence. It is not tax, legal, payment-provider, or accounting advice; verify provider terms and route regulated questions to qualified reviewers.
