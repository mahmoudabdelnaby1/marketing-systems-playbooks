# Salla and Klaviyo Lifecycle Event Mapping

Salla's official help page describes events available through its Klaviyo integration. Verify actual event names and payloads in the connected store before building flows.

| Observed event | Possible operational use | Checks before messaging |
|---|---|---|
| Placed Order | Order confirmation or post-purchase service | Order state, consent, suppression, frequency |
| Ordered Product | Product-specific education or replenishment review | Item identity, actual replenishment cycle, consent |
| Fulfilled Order | Delivery follow-up | Fulfilment state and delivery timing |
| Cancelled Order | Service recovery | Cancellation reason and available support option |
| Refunded Order | Refund status and support | Refund state, policy, customer preference |

Do not add fixed delays, discounts, referral terms, or retention targets without store-specific evidence and approval. See [Salla's Klaviyo guide](https://help.salla.sa/en/article/klaviyo-for-email-marketing/ei4v68ejnkyzov67mzkc0oo6).
