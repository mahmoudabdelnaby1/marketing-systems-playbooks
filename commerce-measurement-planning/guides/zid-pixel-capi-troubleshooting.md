# Zid Event-Tracking Troubleshooting Worksheet

Use current Zid and destination-platform documentation to confirm available integrations, required roles, event names, and fields. Menus and capabilities can vary by account, plan, market, and product updates; the steps below are diagnostic prompts, not claims about every Zid store.

## Connection issues

- Capture the exact error, time, account, integration, and steps that produced it.
- Confirm the connecting user has the role required by the current integration flow.
- Check that the intended business, ad account, pixel/dataset, and catalog are selected and accessible.
- Review connection status in both Zid and the destination platform; record the visible evidence.
- If access appears correct, use the current official support path and preserve the error details. Do not create duplicate assets as a first response.

## Missing or inconsistent events

1. Reproduce with a controlled test action and note its timestamp and order/reference ID.
2. Inspect browser events and server receipts separately; a successful HTTP response alone does not prove correct event data.
3. Compare event name, order identifier, value, currency, timestamp, consent state, and any deduplication identifier with the source order.
4. Check browser console/network diagnostics, tag firing conditions, recent theme/integration changes, retries, and duplicate sends.
5. Reconcile against backend orders with the same timezone, event definition, and date window. Note attribution limitations separately.

## Record findings

| Test | Browser observation | Server observation | Order-system match | Evidence / next action |
|---|---|---|---|---|
| [test action] | [result] | [result] | [result] | [timestamp, issue] |

Avoid fixed match-rate thresholds or claims that a particular cause is “the top reason” without account-specific evidence. Document the current official sources and the date checked.

