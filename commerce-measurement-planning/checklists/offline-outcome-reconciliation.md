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

A reported event or platform-attributed conversion is not, by itself, proof of incrementality or collected revenue. This checklist does not replace legal, privacy, or platform-policy review.
