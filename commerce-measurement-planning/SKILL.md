---
name: salla-zid-shopify-capi-gtm-kit
description: "Plans and troubleshoots e-commerce event tracking across Salla, Zid, Shopify, and WooCommerce. Uses current platform documentation, consent-aware data handling, test events, and order reconciliation; does not promise match rates or attributed revenue."
---

# E-commerce Event Tracking Diagnostic Workflow

Use this guide to investigate browser pixels, server events, consent, event identifiers, and order reconciliation. Platform interfaces and features change; verify the merchant's current plan and the relevant official documentation before giving platform-specific steps.

## 1. Establish the measurement question

- Identify the platform, plan, storefront domain, markets, channels, and exact business question.
- Confirm which event matters and how the merchant defines a real outcome (for example, a paid order versus a placed COD order).
- Identify consent requirements, privacy notices, retention limits, and who is allowed to access customer data.
- Record the date range, timezone, attribution settings, and source of each reported number.

## 2. Map the existing event path

Document the customer action, browser event, server event, event name, event identifier, value, currency, source, consent state, and system of record. Do not assume a named field or integration is available on every plan. Use test mode and a controlled test transaction where possible.

## 3. Diagnose discrepancies

Compare storefront/browser observations, server receipts, ad-platform diagnostics, and backend orders for the same period and definition. Check consent behavior, duplicate firing, missing or inconsistent identifiers, currency/value mapping, timestamps, retries, and recent theme or integration changes. Treat platform match or attribution diagnostics as signals, not proof that all orders were recorded or caused by ads.

## 4. Recommend a scoped change

Prefer the least complex supported integration. Change one element at a time, document a rollback path, and validate in a test environment before production. Use only fields the destination API currently documents and the merchant is permitted to process. Normalize data only when the source meaning is known; hash identifiers as required by the platform and applicable policy.

## 5. Verify and report

For each event, report what was observed, where it was observed, evidence and timestamps, unresolved gaps, and the next check. Avoid universal match-rate targets, guaranteed attribution, or fixed performance claims. Do not describe the implementation as complete until the merchant has completed an appropriate end-to-end test and reconciliation.

## Output

| Event | Browser | Server | Identifier / deduplication | Backend outcome | Evidence and open issue |
|---|---|---|---|---|---|
| [event] | [observed / not observed] | [observed / not observed] | [observed / unknown] | [count or not checked] | [source, time, issue] |

When recommending a platform-specific action, link the current official documentation and state the exact account, plan, and date checked.


