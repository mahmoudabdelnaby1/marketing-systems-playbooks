# E-commerce Event Tracking: Implementation and QA Kit

A practical set of schemas, checklists, and platform notes for planning and diagnosing browser and server-side commerce events across storefronts and advertising platforms.

## Included

- [`SKILL.md`](SKILL.md): diagnostic workflow.
- [`schemas/ecommerce-capi-event-schema.json`](schemas/ecommerce-capi-event-schema.json): event-mapping worksheet; populate it from current platform documentation.
- [`checklists/`](checklists/): pre-launch and deduplication review prompts.
- [`guides/`](guides/): platform implementation notes.
- [`templates/event-tracking-audit-report-template.md`](templates/event-tracking-audit-report-template.md): blank evidence and reconciliation report template.

## Use safely

Map the actual storefront data layer, consent state, event IDs, timestamps, currency, and order lifecycle. Test events in each platform's diagnostics, reconcile against backend orders, and document known gaps. Hashing or transmitting identifiers must follow the relevant platform documentation and applicable privacy requirements. Do not assume server-side tracking restores all lost signals or improves match quality by a fixed amount.

Platform interfaces and APIs change. Verify current official documentation before implementation. This kit is an engineering aid, not a guarantee of delivery, attribution, or compliance.

For GA4 source/medium investigations and commerce reconciliation, use [`GA4 Source and Commerce Reconciliation Review`](checklists/ga4-source-reconciliation.md). It emphasizes non-destructive checks and distinguishes analytics events from store orders.


For inquiries and offline outcomes that later become orders or other business events, use the [Offline Outcome Reconciliation](checklists/offline-outcome-reconciliation.md). It complements setup guidance and does not authorize data uploads.
