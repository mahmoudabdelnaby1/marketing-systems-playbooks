# Outbound Permission and Suppression Review

Use this record before sending a permission-based marketing email or enabling an automated outbound sequence. It organizes operational evidence; it does not determine whether a campaign is lawful in every jurisdiction.

## Campaign and audience

- Campaign/sequence owner and approver:
- Sending identity, provider, and message type:
- Intended recipients and markets:
- Recipient-selection rule and business purpose:
- Data source, collection date, source terms, and permitted-use review:
- Permission/relationship basis recorded for each audience segment, with evidence location:
- Local legal/privacy reviewer and review date, where required:

## Suppression and recipient controls

- Suppression list owner, last sync time, and source systems:
- Unsubscribed, bounced, complained, and do-not-contact records excluded:
- Suppression behavior tested for this sequence and connected systems:
- Reply handling, opt-out route, and responsible team:
- Frequency, duplicate-contact, and cross-campaign collision controls:
- Personal-data minimization, retention, and access controls:

## Message and operations

- From identity, subject, purpose, and truthful content reviewed:
- Required unsubscribe mechanism for the provider, message class, and volume verified against current official requirements:
- Sender authentication and alignment evidence linked to the technical review:
- Automation stop conditions, monitoring owner, and incident contact:
- Test recipient, timestamp, provider, and observed headers/results:
- Known unknowns, launch decision, and next review date:

## Decision record

Choose one: `Ready for authorized human approval` · `Hold for evidence or control gap` · `Do not send`.

List each unresolved issue with its owner and due date. A valid SPF/DKIM/DMARC result does not establish recipient permission, and permission records do not establish inbox placement. Do not use purchased, scraped, or inferred contact lists unless their source, terms, and lawful use have been specifically reviewed for the relevant market.

### Official technical reference

[Gmail sender guidelines](https://support.google.com/mail/answer/81126) describe authentication and unsubscribe requirements for applicable senders and message types. Check the current provider and market requirements for the actual campaign. This template is an operational aid, not legal advice or a deliverability guarantee.
