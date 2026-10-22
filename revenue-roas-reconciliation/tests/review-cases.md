# Reconciliation Review Cases

Use these cases to check that a report preserves definitions and uncertainty. They are logic checks, not measured examples or universal platform behavior.

1. **Refund after reporting period:** State whether the report is order-date or refund-date based. Show any timing shift; do not silently rewrite a past export.
2. **COD order:** Keep placed, delivered, and collected statuses separate. Do not count an attempted delivery as collected revenue.
3. **Cross-platform overlap:** Preserve each platform's attributed result separately. A shared order may appear in more than one platform's report.
4. **Currency conversion:** Record source currency, rate provider/date, and rounding rule. Recalculate only under the declared basis.
5. **Unmatched row:** Assign a review status and evidence owner. Do not infer fraud, tracking failure, or channel causality from the absence of a match.
6. **Different timezones or windows:** Align or disclose the difference before comparing. A remaining difference may be unresolved.
7. **Sensitive identifiers:** Keep row-level exports in a restricted environment. Publish aggregate results only after a privacy and permission review.

Pass condition: another reviewer can reproduce the comparison from the declared sources and choices, and can distinguish measured facts from explanations and unknowns.
