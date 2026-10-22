# WhatsApp Business Platform Cost Model

A local, editable planning model for estimating message charges from rates and volumes entered by the user. It contains no embedded Meta or provider price card. Retrieve current market/category rates and any tier rules from the official pricing sources, record the market, billing currency, and retrieval date, then enter the applicable quantities.

## Use it when

A team needs a transparent estimate for WhatsApp Business Platform message costs and wants to separate Meta charges from provider fees, taxes, and other commercial terms.

## Prepare

- The recipient market and billing currency.
- Current official Meta rates and volume-tier rules for the relevant category and period.
- Forecast delivered-message quantities, split by category and applicable pricing tier.
- The portion that is explicitly no-charge under the current official rules, if applicable.
- Provider charges, applicable taxes, and any approved FX conversion entered as separate inputs.

## Included

- `index.html` / `index-ar.html`: English and Arabic offline-capable, browser-local calculators. They store no data and send no form contents anywhere.
- `SKILL.md`: reusable procedure for building and reviewing a cost estimate.
- `templates/cost-model-inputs.csv`: blank rate, volume, source, fee, and assumption register.

## Calculation

For each entered pricing line, the tool calculates:

`billable delivered messages = max(delivered messages − explicitly eligible no-charge messages, 0)`

`Meta estimate = billable delivered messages × entered unit rate`

It then adds user-entered provider fees and calculates tax only from the separately entered, user-confirmed taxable base and rate. Add separate rows for each market/category/tier rate that applies. This is a planning estimate, not an invoice or quote.

## Workflow

1. Select one recipient market and billing currency for the estimate.
2. Open Meta's official pricing page and rate cards; enter each applicable category/tier as a separate line and record the date and source in the notes/CSV.
3. Use delivered-message volume, not sent volume. Enter zero-rated volume only after confirming eligibility under the current official rules.
4. Add the provider's separate monthly, per-message, setup, or other fees from the relevant contract. Do not assume a BSP margin or included service.
5. Enter tax only after confirming how it applies to the relevant charges. Keep currency conversion outside the model unless the rate and date are documented.
6. Review the assumptions with the account/provider owner before budgeting; compare estimates with an actual invoice after the period closes.

## Boundaries

- Meta rates, categories, tier thresholds, and free/no-charge conditions can change. The official pricing page and current rate cards control; this repo does not supply a hardcoded rate.
- Rates may depend on recipient market, category, message delivery, and tier. Split lines when different rules or rates apply.
- A user's free-entry-point eligibility or other no-charge quantity must be identified from the applicable current rule and actual messaging records. Do not simply assume a percentage is free.
- Provider pricing, taxes, currency conversion, account terms, and invoice treatment are separate from this Meta-only calculation and must be entered from current evidence.
- No output from this model is financial, tax, legal, or platform approval advice.

## Official source

- [WhatsApp Business Platform pricing and rate cards](https://whatsappbusiness.com/products/platform-pricing/)

The official page describes per-delivered-message pricing, market/category rates, four message categories, volume tiers for utility and authentication, and specific no-charge cases. Check the live page and linked rate card before each estimate.


Neither language version contains a prefilled rate card. The corresponding public calculator pages are available from the portfolio guide.
