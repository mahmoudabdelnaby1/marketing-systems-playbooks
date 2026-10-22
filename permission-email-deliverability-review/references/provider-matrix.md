# Provider Requirements — Verification Matrix

**Reviewed:** 2026-10-22. Links below are the governing references to re-check at the time of a review. This matrix is a navigation aid, not a substitute for the full current requirements.

| Destination | Scope to check in current guidance | Source |
|---|---|---|
| Gmail personal accounts | All senders: SPF or DKIM minimum. Senders exceeding 5,000 messages/day to Gmail personal accounts have additional SPF, DKIM, DMARC, alignment, and marketing/subscribed-message unsubscribe requirements. Google recommends spam rates below 0.10% and avoiding 0.30% or higher. | [Gmail sender guidelines](https://support.google.com/mail/answer/81126?hl=en) and [FAQ](https://support.google.com/mail/answer/14229414?hl=en) |
| Yahoo Mail | Separate requirements for all senders and bulk senders. Bulk guidance includes SPF and DKIM, DMARC with at least p=none and alignment, easy unsubscribe for marketing/subscribed mail, and complaint-rate guidance. Confirm the current definition and mechanics on Yahoo's site. | [Yahoo Sender Best Practices](https://senders.yahooinc.com/best-practices/) |
| Outlook.com consumer services | Microsoft has published requirements for high-volume senders to consumer Outlook.com services. Scope those requirements to the covered consumer services and volume classification; do not apply them automatically to organizational Microsoft 365 tenants. | [Microsoft Outlook.com high-volume sender update](https://techcommunity.microsoft.com/blog/microsoftdefenderforoffice365blog/strengthening-email-ecosystem-outlook%E2%80%99s-new-requirements-for-high%E2%80%90volume-senders/4399730) |
| DMARC standard | Use the current IETF specification. RFC 9989 (May 2026) obsoletes RFC 7489 and RFC 9091. | [RFC 9989](https://www.rfc-editor.org/rfc/rfc9989.html) |
| One-click unsubscribe | Check the applicable provider and message class. Gmail references RFC 8058 for one-click unsubscribe; body links and header mechanics are separate checks. | [RFC 8058](https://www.rfc-editor.org/rfc/rfc8058.html), plus provider guidance above |

## Interpretation guardrails

- Classify by receiving service, sender volume to that service, and message type; total program volume alone can mislead.
- A configured SPF, DKIM, or DMARC record is not proof that an individual message passes or aligns.
- Report provider-specific thresholds exactly and with the source. Do not turn a recommendation into a universal guarantee or infer inbox placement from authentication.
- Do not mix Gmail, Yahoo, Outlook.com consumer, and Microsoft 365 organizational policy into one generic checklist.
