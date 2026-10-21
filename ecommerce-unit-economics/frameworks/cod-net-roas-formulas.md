# Order-Level Unit Economics Formulas

This framework makes no regional assumptions. Populate it with current store, tax, courier, payment, and advertising data. Keep each input's source and date alongside the calculation.

## Inputs

| Symbol | Input | Unit / source |
|---|---|---|
| `AOV_gross` | Average order value before refunds | Store orders |
| `tax_rate` | Applicable tax rate and treatment | Accountant/current authority guidance |
| `COGS` | Product cost charged to a delivered and retained order | Inventory/accounting records |
| `COGS_if_lost` | Non-recoverable product cost on a failed order; use zero when inventory is fully recoverable | Inventory/accounting records |
| `ship_out` | Outbound fulfillment cost | Current courier contract |
| `ship_return` | Return/failed-delivery cost | Current courier contract |
| `payment_fee` | Weighted provider/COD fee | Current provider contracts |
| `p_delivered` | Share of placed orders delivered and retained (fraction from 0 to 1) | Store order data, defined period |
| `ad_cost_per_order` | Advertising cost per placed order | Ad account + reconciled order data |

## Equations

Net order value (if tax is included in the reported value and is excluded from revenue for this model):

`AOV_net = AOV_gross / (1 + tax_rate)`

Expected contribution per placed order:

`expected_contribution = p_delivered × (AOV_net − COGS − ship_out − payment_fee) − (1 − p_delivered) × (COGS_if_lost + ship_out + ship_return + other_failure_costs)`

Break-even advertising cost per placed order:

`break_even_CPA = expected_contribution`

Net return on ad spend for the selected attribution and reconciliation method:

`net_ROAS = reconciled_net_revenue / ad_spend`

Adjust the terms to match accounting treatment and whether costs are charged on failed orders. Do not count the same fee in both delivered and failed-order costs. If payment methods have materially different delivery outcomes, calculate each method separately and weight by the observed mix.

## Interpretation cautions

- Define whether the denominator is placed, confirmed, shipped, delivered, or retained orders.
- Align attribution window, timezone, currency, and order dates before comparing ad platforms with store data.
- Separate platform-reported conversions from backend orders and settled cash.
- Use scenario analysis to understand sensitivity; scenarios are not forecasts or regional benchmarks.
- Confirm tax and accounting treatment with a qualified professional.


