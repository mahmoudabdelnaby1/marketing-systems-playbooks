# WhatsApp-Assisted Order Measurement: Design Worksheet

Some customer journeys move from an ad or storefront into a WhatsApp conversation. This worksheet helps a merchant decide whether and how to measure that path. It does not assume how common the behavior is, that browser tracking misses every order, or that a reported order was caused by an ad.

## Map the journey

```text
Ad or referral → storefront → customer chooses WhatsApp → conversation
→ order system records outcome → eligible measurement event (if permitted)
```

For each handoff, identify the system, owner, timestamp, consent state, and data retained. Prefer an optional, non-sensitive reference that the customer can remove; do not place personal data or ad identifiers into a public message.

## Measurement decisions

- Define the business outcome precisely: inquiry, confirmed order, paid order, fulfilled order, or another status.
- Decide which source is authoritative for each field and how the order is matched to a conversation.
- Use current official destination API documentation for event names, action source, required fields, retention, and consent rules.
- Minimize data, restrict access, and document deletion/retention. Do not collect or send IP addresses, phone numbers, message contents, or click identifiers without a documented lawful and technical basis.
- Use a stable event identifier only where the destination's current documentation supports it; test duplicate and retry behavior.
- Reconcile reported events to backend orders and disclose unmatched records and attribution limits.

## Test record

| Reference | Conversation outcome | Backend order status | Destination event | Consent / evidence | Reconciliation |
|---|---|---|---|---|---|
| [non-sensitive test ID] | [outcome] | [status] | [not sent / test receipt] | [details] | [matched / unmatched] |

Do not copy production customer data into examples. Use synthetic IDs and values in public documentation.

