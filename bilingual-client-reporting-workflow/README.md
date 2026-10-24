# Bilingual Client Reporting Workflow

A human-reviewed workflow for turning approved marketing data into a concise client report in Arabic, English, or both. It keeps source facts, interpretation, and recommended action distinct so the report can be checked before it is shared.

## Use it when

A marketing team needs a consistent monthly or campaign report for a client, leadership team, or cross-market stakeholder group, especially when the report needs Arabic and English versions.

This is a reporting workflow and a set of templates. It is not an automated CSV parser, dashboard, attribution model, or guarantee of faster reporting or better campaign results.

## Prepare

- The reporting question and decision the reader needs to make.
- The reporting period, timezone, currency, comparison period, and any unequal date coverage.
- Approved aggregate exports or reports, with each source and its definitions recorded.
- The business outcome definition, platform attribution settings, and system of record relevant to the question.
- Audience, language order, Arabic register, terminology, and an accountable reviewer.
- A restricted workspace for any confidential source files. Do not place customer-level data, credentials, or unapproved exports in public repositories or AI prompts.

## Workflow

1. **Agree on the question.** Define the business decision, audience, outcome, period, and scope before selecting headline metrics.
2. **Register the sources.** Record source owner, export time, timezone, filters, currency, metric definitions, and known limitations. Keep platform-attributed results separate from store, CRM, finance, or operational records.
3. **Check comparability.** Confirm date coverage, status filters, event definitions, and calculation basis. If sources or periods are not comparable, show the limitation instead of forcing a comparison.
4. **Recalculate the reported figures.** Recheck totals, rates, changes, currency formatting, and rounding against the source. An equal count across two systems does not by itself prove tracking is correct or attribution is complete.
5. **Write in three layers.** Mark each statement as a **fact** supported by the stated source, an **interpretation** that explains a possible mechanism, or a **recommendation** with an owner and next review point. Do not present a hypothesis as a verified cause.
6. **Create the language versions.** Preserve the same figures, scope, uncertainty, and decision in each language. Adapt phrasing to the intended audience; do not strengthen a claim while localizing it.
7. **Review and release.** Use the checklist and cases in this toolkit. Obtain business-owner approval for recommendations and a qualified language review when the audience or register requires it.

## Included

- `SKILL.md` — instructions for an AI-assisted drafting workflow using approved, minimized inputs.
- `templates/report-brief.md` — a source, scope, and decision brief to complete before drafting.
- `templates/client-report-ar-en.md` — a reusable bilingual report structure.
- `tests/report-review-cases.md` — review cases that catch common reporting and translation failures.

## Boundaries

- A platform conversion count, analytics event, CRM stage, and collected order are different measures unless their definitions and records establish otherwise.
- Cross-platform equality is not proof of tracking accuracy; investigate event definitions, attribution windows, delays, deduplication, and source records.
- Month-over-month movement is descriptive unless a suitable design supports a causal claim. Do not attribute a change to a campaign solely because it followed the campaign.
- This workflow does not provide accounting, legal, privacy, or statistical advice and does not replace the relevant owner or specialist.
- Do not copy universal alert thresholds from this guide. Set decision limits from the business question, account history, measurement quality, and available volume, and record who approved them.

## Related playbooks

- [Revenue and ROAS Reconciliation](../revenue-roas-reconciliation/README.md) — compare platform-reported results with store, payment, fulfilment, and finance records.
- [Marketing Incrementality Test Design](../mena-incrementality-test-designer/README.md) — design a controlled test when the question is whether marketing caused additional outcomes.

For cross-functional launch checks related to this toolkit, see the [Marketing Workflow QA & Evidence Gates](../marketing-workflow-qa-gates/README.md#10-reporting--evidence-governance).
