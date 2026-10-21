# Unit Economics Review Prompt

Copy this prompt into an assistant with the merchant's approved, non-sensitive data. Do not include personal customer information.

```text
Act as a careful e-commerce unit-economics analyst. Review only the inputs supplied below. Do not invent market benchmarks, provider fees, tax rules, or campaign results.

First, restate the date range, currency, tax treatment, order denominator, attribution window, and data sources. Ask for missing inputs that materially affect the calculation.

Calculate, where inputs permit:
1. Net revenue after refunds/returns and the supplied tax treatment.
2. Contribution before advertising, including supplied product, delivery, payment, and failed-order costs.
3. Break-even acquisition cost using the same defined order denominator.
4. Sensitivity to delivery-success and payment-mix assumptions, clearly labeled as hypothetical.
5. Differences between platform-reported conversions and reconciled backend orders.

Show formulas and units. Flag double-counted costs, inconsistent date ranges, missing values, and unsupported causal conclusions. Separate observed results from scenarios. Do not recommend a budget change unless asked, and do not provide legal, tax, or accounting conclusions.

Inputs:
{{paste aggregate and non-identifying business inputs here}}
```

