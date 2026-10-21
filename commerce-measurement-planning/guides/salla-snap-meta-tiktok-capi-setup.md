# Salla and Server-Side Event Tracking: Assessment Worksheet

This worksheet helps decide whether to use a platform-native integration or a custom server-side setup. It does not assume a feature, plan entitlement, event schema, setup time, or cost. Verify each item in the merchant's current Salla dashboard and official platform documentation.

## Choose an implementation path

| Check | Native integration | Custom implementation |
|---|---|---|
| Available for the merchant's current plan and market? | [verify] | [verify] |
| Required events and parameters documented? | [verify] | [verify] |
| Consent behavior and privacy responsibilities understood? | [verify] | [verify] |
| Event identifiers and duplicate handling understood? | [verify] | [verify] |
| Owner for maintenance and incident response identified? | [name/role] | [name/role] |

Choose the least complex option that supports the required events and controls. Do not connect two integrations that send the same events until their interaction and deduplication behavior are understood.

## Implementation checklist

1. Record the platform, plan, storefront, destination accounts, markets, and current integration state.
2. Review the current official setup documentation for the selected integration and confirm permissions with an authorized account owner.
3. Map each business action to the platform's documented event name and required fields. Confirm currency, order value, item identifiers, timestamps, and order status from the source system.
4. Define consent handling and minimize customer data. Use only identifiers permitted by the merchant's policies and the destination platform's current requirements.
5. Test in the destination's test or diagnostics mode, including duplicate delivery, retries, cancellation/refund handling, and COD status where relevant.
6. Reconcile a sample of observed events against backend orders using the same dates, timezone, and order definition.
7. Record unresolved issues, owner, rollback plan, and review date before enabling or changing production behavior.

## Verification record

| Item | Evidence / result |
|---|---|
| Official documentation and date checked | [link, date] |
| Test event and timestamp | [details] |
| Browser/server observations | [details] |
| Backend order reconciliation | [details or not checked] |
| Consent and data handling review | [details] |
| Open issue / rollback owner | [details] |

