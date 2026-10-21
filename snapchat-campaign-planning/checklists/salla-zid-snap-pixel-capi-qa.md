# Salla / Zid and Snapchat Tracking Preflight

Use this checklist to document a specific store's setup. Confirm current integration capabilities and required permissions in the official documentation and account UI; do not treat this as a universal launch guarantee.

## Access and configuration

- [ ] Record the store platform, plan, market, Snapchat business/ad account, pixel, and integration path.
- [ ] Confirm the connecting user's required role and asset access in the current platform flow.
- [ ] Confirm the selected assets belong to the intended business and can be accessed by the store integration.
- [ ] Review whether another pixel or server integration already sends the same events.
- [ ] Capture the current documented event names, parameters, consent behavior, and deduplication method.

## Controlled validation

- [ ] Run a controlled test event and record the time and reference.
- [ ] Inspect browser events and server receipts separately.
- [ ] Compare event name, value, currency, item IDs, event identifier, and order status with the source order.
- [ ] Test duplicate delivery and retry behavior where applicable.
- [ ] Reconcile to backend orders for the same date range, timezone, and order definition.
- [ ] Record unresolved issues, owner, and rollback plan before production changes.

Do not promise attributed orders or a particular match rate from a checklist result. Distinguish event receipt, order reconciliation, and ad attribution in the report.

