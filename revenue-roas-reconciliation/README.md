# Revenue and ROAS Reconciliation

A practical workflow for comparing platform-attributed results with store, payment, fulfilment, and finance records. It makes definitions, periods, currencies, order status, refunds, and unmatched records visible; it does not decide which system is universally correct.

## Use it when

Ad platforms, analytics, the store, and finance show different revenue or order totals and a team needs a reproducible comparison before changing budgets or reporting results.

## Prepare

- A defined reporting period, timezone, currency, and business decision.
- Store orders and status history, payment captures or settlements, refunds, and COD delivery/collection outcomes as applicable.
- Platform exports and the attribution settings used for the period.
- A restricted workspace for row-level identifiers. Public examples and shared summaries must not contain customer data.

## Workflow

1. **Agree the metric.** State whether the comparison uses placed orders, captured payments, fulfilled orders, or net collected amounts. Declare tax, shipping, discount, refund, fee, FX, and timing treatment.
2. **Check each source.** Record export time, timezone, currency, filters, event/status definitions, and known omissions.
3. **Match cautiously.** Use an approved, access-controlled order key. Keep unmatched and many-to-many cases visible; never infer a channel from a missing match.
4. **Reconcile.** Compare counts and amounts by status and period. Explain differences only where evidence supports the explanation.
5. **Report limits.** Keep platform attribution separate from business revenue and incrementality. Use the result only for decisions supported by the data.

## Included

- A metric-definition worksheet and declared-choice register.
- A source-field mapping template and reconciliation report.
- Review cases for refunds, COD, currency, timing, duplicate claims, and unmatched records.

## Boundaries

Attribution is a reporting rule, not proof that an ad caused an order. Platform totals may overlap and may use different windows, event sources, and reporting dates. A match does not establish incrementality; see [Marketing Incrementality Test Design](../mena-incrementality-test-designer/README.md). This toolkit is not accounting or tax advice, and it does not prescribe universal match rates or tolerance thresholds.

## Quick start

Use `SKILL.md` for an AI-assisted or analyst-led workflow. Copy the blank templates, declare definitions before calculating, and retain a source trail for every transformed field. Start with aggregate counts if row-level matching is not necessary. See [metric definitions](framework/metric-definitions.md), [source-field map](templates/source-field-map.csv), and [reconciliation report](templates/reconciliation-report.md).

## References

Confirm current platform attribution settings in the relevant platform account and current financial definitions with the business's finance owner. The framework is platform-neutral and makes no claim that one attribution setting is correct for every decision.
