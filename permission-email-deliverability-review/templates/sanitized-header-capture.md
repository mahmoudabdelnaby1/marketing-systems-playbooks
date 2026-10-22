# Sanitized Message Evidence Capture

Capture a message delivered to a mailbox you control or an authorized test account. Do not use a real recipient's mailbox without permission.

## Before sharing

Remove or replace:

- Recipient and personal addresses, names, phone numbers, and message content.
- Message IDs and any provider-specific identifiers that could expose a person or account.
- Authentication tokens, credentials, or tracking URLs containing user identifiers.

Retain only the fields needed to assess authentication, alignment, routing, and unsubscribe behavior. Keep the original in the organization's restricted environment.

## Capture record

| Field | Value |
|---|---|
| Date and time received, with timezone | ___ |
| Sending domain and subdomain | ___ |
| Sending provider / stream | ___ |
| Receiving service / account type | ___ |
| Message class | marketing/subscribed / transactional / other |
| Approximate daily volume to this provider | ___ |
| Visible From domain | ___ |
| SPF result and authenticated domain | ___ |
| DKIM result and signing domain/selector | ___ |
| DMARC result and alignment evidence | ___ |
| List-Unsubscribe header present? | ___ |
| List-Unsubscribe-Post header present? | ___ |
| Test unsubscribe action and result (authorized test only) | ___ |
| Evidence retained by / access location | ___ |

Do not paste the full raw headers or message into a public issue. If exact header review is required, use an approved restricted channel.
