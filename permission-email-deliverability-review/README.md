# Permission-Based Email Deliverability Review

A repeatable technical review for permission-based email programs. It checks sender authentication, alignment, list handling, message headers, and monitoring without promising inbox placement or treating opens as delivery evidence.

## Use it when

A team is investigating spam placement, rejection, authentication warnings, or a sender-domain change, and needs to separate DNS configuration from what a received message actually authenticated.

## Prepare

- Sending domains and subdomains, providers, message types, and recipient mailbox types.
- Current DNS records and a sanitized copy of a representative message's authentication headers.
- Sending volume by recipient provider, not only total program volume.
- Recent provider diagnostics and the exact date/time of the sample.
- A technical owner for DNS/provider changes and a reviewer for permission, privacy, and jurisdiction questions.

Remove recipient addresses, message bodies, tokens, and identifying content before sharing headers. Do not share credentials or mailbox access.

## Review sequence

1. **Scope the rule.** Distinguish marketing/subscribed from transactional mail, Gmail personal accounts from Workspace, Yahoo Mail from other providers, and Outlook.com consumer requirements from organizational Microsoft 365 controls.
2. **Inspect DNS.** Check SPF, DKIM, and DMARC for the actual sending identity. Compare the visible From domain with authenticated domains; note alignment mode and message-specific results.
3. **Inspect a received message.** Read the receiving server's Authentication-Results and relevant List-Unsubscribe headers. A published DNS record alone does not show that a given message passed.
4. **Review sending and list controls.** Confirm permission source, suppression, unsubscribe processing, bounce/complaint monitoring, and separation of message streams.
5. **Report evidence and unknowns.** State the message/provider/date tested, evidence, what is not verified, and who owns each follow-up.

## Included

A provider-specific reference matrix, sanitized header capture sheet, diagnostic report, and review cases.

## Boundaries

Authentication is not a guarantee of inbox placement. A single sample does not establish delivery across providers or time. Provider rules change; re-check current official guidance before acting. This is a technical review aid, not legal advice, a DNS change service, or a permission audit.

## Start here

Use `SKILL.md` for the review sequence. Use [the provider matrix](references/provider-matrix.md), [the capture template](templates/sanitized-header-capture.md), and [the report template](templates/review-report.md). Make no DNS or sending change based solely on this checklist; have the domain/provider owner validate the proposed change.

For recipient eligibility and automated outreach controls, use the separate [Outbound Permission and Suppression Review](templates/outbound-permission-and-suppression-review.md). It complements the technical deliverability review; it does not replace jurisdiction-specific legal review.

For cross-functional launch checks related to this toolkit, see the [Marketing Workflow QA & Evidence Gates](../marketing-workflow-qa-gates/README.md#07-email-lifecycle--automation).
