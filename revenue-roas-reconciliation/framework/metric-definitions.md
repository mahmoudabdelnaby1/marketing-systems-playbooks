# Metric Definitions and Reconciliation Choices

Use one declared definition per comparison. Do not silently compare unlike values.

## 1. Define the business event

| Event | Example definition | Check before use |
|---|---|---|
| Order placed | An order record was created | May include unpaid, cancelled, duplicate, or test orders unless excluded |
| Payment captured | A payment provider confirms capture | A capture may later be refunded, disputed, or reversed |
| Fulfilled | Goods or service were delivered under the business's status rules | Status definitions vary by store and operation |
| Collected | Funds were received and reconciled to the order | COD may require delivery and collection confirmation |
| Net collected | Collected amount less refunds, reversals, or other declared adjustments | State which adjustment dates and fees are included |

These are distinct views, not a universal ranking. A finance report may use a recognized accounting basis that differs from an operational cash view.

## 2. Declare the comparison basis

Record the reporting period, timezone, currency, tax treatment, discount basis, shipping treatment, refund and chargeback treatment, payment fees, FX source/date, and order-status filters. Record each platform's reporting window, event source, attribution setting, and export timestamp separately. Do not assume settings or definitions remained constant during the period.

## 3. Keep metric families separate

- **Store or finance amount:** amount under the business's declared order, payment, or accounting definition.
- **Platform-attributed amount:** amount reported by one advertising platform under its own configuration and reporting rules.
- **Analytics amount:** amount collected by an analytics system under its event, consent, and processing configuration.
- **Incremental outcome:** estimated additional outcome supported by an appropriate experiment or causal design, with stated assumptions and uncertainty.

Do not sum cross-platform attributed revenue and label it unique revenue. A single order may appear in multiple systems. Do not label every unmatched row as tracking failure, fraud, or platform error; investigate and keep unknowns unknown.

## 4. Matching and tolerance

Use an approved, access-controlled key only when the owner has a documented purpose and lawful basis. A matching rule must state key, time window, currency conversion, one-to-one or many-to-one handling, and exception treatment. Choose tolerances from source precision and the business decision before reviewing results; do not tune a tolerance to force agreement. Keep row-level data restricted and share aggregate outputs.

## 5. Formulas (only after definitions are fixed)

```text
net amount = declared gross amount - included refunds - included reversals
platform ROAS = one platform's attributed conversion value / that platform's spend
business efficiency ratio = declared business outcome amount / declared media cost
```

These ratios are not interchangeable. State numerator, denominator, period, currency, and source alongside each result. A business efficiency ratio is not automatically incremental return.
