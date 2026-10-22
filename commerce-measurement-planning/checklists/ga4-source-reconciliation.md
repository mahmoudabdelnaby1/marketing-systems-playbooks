# GA4 Source and Commerce Reconciliation Review

Use this checklist to investigate a source/medium or commerce-reporting change without treating analytics reports as the store ledger.

## Define the comparison

- Record property, data stream, report/exploration, date range, timezone, and filters.
- State the exact dimension, metric, attribution setting, and event definitions being compared.
- Note consent behavior, referral exclusions, cross-domain setup, UTMs, and campaign naming rules in scope.
- Keep a copy of the current configuration and the source export before any change.

## Validate the path

- Use a controlled test journey to confirm landing-page URL parameters and expected events.
- Check event parameters, currency, transaction/order identifiers, deduplication, and domain transitions.
- Compare analytics transactions with store orders for the same period and status definitions.
- Separate observed missing/duplicate data from hypotheses about why it happened.
- Do not use a permanent traffic filter to “clean” data until its effect is previewed and the data owner approves a reversible plan.

## Reconcile and report

- Compare like-for-like periods and segments; record known sampling, consent, and processing limitations.
- Distinguish platform-attributed conversions, analytics events, store orders, completed payments, and fulfilled orders.
- Record source, export date, calculation, reviewer, discrepancy, and follow-up owner.
- Recheck after changes to consent, tagging, checkout, domains, or analytics settings.

This checklist does not establish the true source of every order and does not replace backend order records or current Google Analytics documentation.
