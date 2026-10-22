# Email Sender Readiness Checklist

A technical pre-send review for an email program. It does not determine legal permission to contact recipients or guarantee inbox placement.

## Domain and sending setup

- Confirm the sending domain and responsible technical owner.
- Check SPF, DKIM, and DMARC configuration using current provider instructions.
- Verify the visible From address, reply path, sending service, and alignment expected by the provider.
- Confirm unsubscribe handling, suppression processing, bounce handling, and complaint monitoring in the sending platform.
- Send test messages to representative clients and inspect headers, links, images, and Arabic RTL rendering.
- Confirm the production sending flow does not accidentally include internal/test recipients or suppressed contacts.

## List and message controls

- Identify the source and permitted purpose for each audience segment; route consent and jurisdiction questions to qualified counsel.
- Check exclusions, frequency rules, preference options, and unsubscribe experience.
- Validate every link, CTA destination, personalization fallback, and localized version.
- Assign a monitor for bounces, complaints, delivery, clicks, and downstream outcomes; define a stop/escalation path.
- Record the sending tool, configuration evidence, reviewer, and date. Recheck after domain, provider, or policy changes.

Do not import purchased or scraped lists based on this checklist. This is a technical readiness aid, not legal advice or a guarantee of deliverability.
