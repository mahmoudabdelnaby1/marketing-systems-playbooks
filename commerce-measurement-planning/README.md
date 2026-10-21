# Commerce Measurement Planning Kit

A platform-agnostic planning and QA framework for mapping ecommerce events across storefront, analytics, and advertising destinations. It does not include a production integration or claim that a pixel/CAPI setup is complete.

## Included

- `event-map.csv` — event and data-flow inventory.
- `prelaunch-checklist.md` — review before and after implementation.
- `architecture-notes.md` — consent, data minimization, deduplication, and reconciliation considerations.

## Workflow

1. Map the business event and authoritative source (store, CRM, or backend).
2. Identify which destinations need the event and what fields are strictly necessary.
3. Review consent, privacy notice, retention, access, and applicable platform terms with the responsible owner.
4. Implement in the relevant platform/account using current official documentation and an authorized technical owner.
5. Validate in test mode, then reconcile observed events against the source system before relying on reports.

Do not assume that hashing makes an identifier anonymous. Have the responsible privacy owner review purpose, consent or other applicable basis, retention, and access before transmitting customer or click identifiers.