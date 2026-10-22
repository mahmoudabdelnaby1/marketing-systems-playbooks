# Offline Outcome Reconciliation

Use this checklist when an inquiry, WhatsApp conversation, phone call, or store interaction later becomes an order or another business outcome. It complements event setup and does not determine whether data may be uploaded to an advertising platform.

## Define the outcome and source

- Choose one outcome (for example: qualified inquiry, confirmed order, collected order, or completed appointment) and define who records it.
- Document the source system, event timestamp, status history, timezone, and deduplication rule.
- Keep inquiry, order, payment, fulfilment, and collection as distinct stages.
- Reconcile with aggregate totals first; row-level joins require a documented purpose, approved access, and retention controls.

## Review the handoff

- Map the source record, CRM/store status, responsible owner, and approved destination event.
- Check the destination's current official documentation for event name, action source, required fields, retention, permitted data, consent handling, and retries.
- Do not copy message contents, phone numbers, email addresses, click IDs, or other identifiers into prompts, public files, or reports.
- Use identifiers only through an authorized integration and its approved privacy/security design; hashing alone does not make data anonymous or establish permission.
- Record duplicate, late, rejected, unmatched, and corrected events without assigning a cause until evidence supports it.

## Release and reconciliation record

| Check | Evidence / owner |
|---|---|
| Outcome definition and source owner | ___ |
| Authorized data path and destination configuration | ___ |
| Test event receipt and duplicate/retry behavior | ___ |
| Aggregate reconciliation period and timezone | ___ |
| Unmatched or rejected events and investigation status | ___ |
| Retention/deletion and access review | ___ |

## Team handoff and operating cadence

Agree who owns each step before the first import or report:

| Owner | Responsibility | Record / timing |
|---|---|---|
| Marketing | Campaign, market, reporting-period, and source-spend definitions | Agreed export and reporting cadence: ___ |
| Sales / customer operations | Outcome status, status-change time, and source-system record | Update cadence and required fields: ___ |
| Analytics / implementation | Event mapping, deduplication, import behavior, and discrepancy investigation | Test evidence and change log: ___ |
| Finance / business owner | Revenue, payment, refund, currency, and collection definitions | Definition approver and review date: ___ |

At each review, reconcile aggregate counts and values first; then assign owners and due dates for late, rejected, duplicate, unmatched, and unknown records. Keep the comparison period, timezone, outcome-stage definitions, and system of record explicit. Do not force uncertain records into a channel or outcome category to make totals agree. Revisit definitions when the business process or data path changes.

Use row-level matching only when aggregate reconciliation cannot answer the decision and the business has approved the purpose, access, retention, and destination-specific data handling. A consent field or hashed identifier by itself does not establish permission to upload data.

A reported event or platform-attributed conversion is not, by itself, proof of incrementality or collected revenue. This checklist does not replace legal, privacy, or platform-policy review.
