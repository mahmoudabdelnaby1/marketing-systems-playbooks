---
name: bilingual-client-reporting-workflow
description: Draft a human-reviewed Arabic and/or English marketing report from approved aggregate source data. Use when preparing a recurring client or leadership report. Do not infer causation from attribution, merge incompatible metrics, invent missing figures, or request unnecessary customer-level data.
license: MIT
---

# Bilingual Client Reporting Workflow

## Role

Prepare a traceable first draft. A responsible human reviews calculations, interpretation, recommendations, confidentiality, and language before delivery. This skill does not generate or verify data automatically.

## Before drafting

1. Read the completed `templates/report-brief.md`.
2. Confirm the authorized data scope. Prefer aggregated exports. Never ask the user to paste customer names, phone numbers, email addresses, message contents, access tokens, or credentials. If row-level data is essential, pause for an approved restricted workflow and use only the minimum fields required.
3. Confirm the report period, timezone, currency, source definitions, and audience. If any of these are missing and could change a conclusion, ask for clarification or label the item unresolved.
4. Identify the business decision. Do not select metrics only because they look favorable.

## Drafting sequence

1. Summarize the decision and reporting scope.
2. Build a source register with the source, metric definition, date coverage, filters, currency, and limitations.
3. Report factual figures only when they are present in approved source material. Preserve the supplied precision and show formulas for derived rates or period changes.
4. Separate the report into:
   - **Fact:** directly supported by a named source and period.
   - **Interpretation:** a plausible explanation, explicitly marked as unconfirmed unless evidence establishes it.
   - **Recommendation:** a proposed action, its owner, review date, and a measurable decision rule agreed for this case.
5. Keep platform attribution, analytics events, CRM outcomes, and business-record outcomes separate unless the source definitions justify a comparison. Equal totals do not prove that systems match or that there is no tracking gap.
6. If periods differ in length, sources change definitions, data is delayed, or a metric is missing, state the limitation. Do not silently adjust, fill, or normalize it.
7. Produce the requested language version(s). Keep claims, figures, qualifications, and recommendations equivalent. Use the specified market register; do not label dialect as native or locally approved without a qualified reviewer.
8. Complete `templates/client-report-ar-en.md` and apply `tests/report-review-cases.md` before delivery.

## Never

- Invent values, trends, explanations, client details, or actions.
- Present a correlation, before/after change, platform-attributed result, or matching count as causal proof.
- Sum platform-reported conversions or revenue as unique business outcomes without a defensible deduplication method.
- Apply a generic performance threshold as a universal stop, scale, or budget rule.
- Hide an unfavorable result, unresolved mismatch, limitation, or missing baseline.
- Translate an unverified claim into a stronger claim in the other language.
- Describe a report as machine-verified, audited, or approved unless the stated process and evidence support that label.
