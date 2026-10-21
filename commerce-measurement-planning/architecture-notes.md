# Architecture and data-handling notes

A typical measurement path is:

`store or CRM source → consent and eligibility checks → event transformation → authorized destination(s) → reconciliation`

This is a conceptual map, not executable implementation guidance. Each ecommerce platform and ad destination has its own current API, event, consent, and retention requirements.

## Design questions

- Which system is authoritative for order, payment, delivery, refund, and cancellation status?
- Is the event browser-originated, server-originated, or both? How are duplicates handled?
- Which identifiers are truly needed for the stated measurement purpose?
- How are consent choices propagated to tags and server-side systems?
- Who can access event payloads and credentials, and how long are they retained?
- How will test events be distinguished from production events?
- How will reported conversions be reconciled to source-system outcomes?

Do not use real personal data in public examples. Use synthetic values and never commit secrets, customer records, raw click IDs, email addresses, phone numbers, or IP addresses.