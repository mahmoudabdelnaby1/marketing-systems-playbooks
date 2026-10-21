# Event Tracking Pre-Launch Review

Use this checklist for the specific storefront, destination, and integration under review. Event names, identifiers, data fields, diagnostics, permissions, and timing differ across platforms and can change. Confirm requirements in current official documentation before implementation.

## Scope and current state

- [ ] Record platform, plan, storefront, markets, destination accounts, and integration owner.
- [ ] List every active browser tag, native integration, server integration, and source of order data.
- [ ] Define the business outcome and order status being measured (for example, placed, confirmed, paid, or fulfilled).
- [ ] Record consent state, data minimization, access, retention, and deletion requirements.
- [ ] Link the official documentation and date checked for each destination.

## Test and reconcile

- [ ] Run a controlled test event and record its timestamp and non-sensitive reference.
- [ ] Observe browser events, server receipts, and destination diagnostics separately.
- [ ] Check event name, identifier, value, currency, item references, timestamp, and consent state against current documentation and the source order.
- [ ] Check for duplicate sends, retries, missing values, and changes introduced by recent theme or integration updates.
- [ ] Reconcile against backend orders using the same date range, timezone, currency, and order definition.
- [ ] Document unresolved issues, rollback steps, and the person responsible before changing production.

## Findings

| Event / action | Browser evidence | Server evidence | Order reconciliation | Issue / next step |
|---|---|---|---|---|
| [action] | [source and time] | [source and time] | [matched / unmatched / not checked] | [detail] |

Do not treat a successful test receipt as proof of complete tracking, attribution, or business impact. Do not use universal match-rate or delivery-time thresholds.

