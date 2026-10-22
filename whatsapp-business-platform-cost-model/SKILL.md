---
name: whatsapp-business-platform-cost-model
description: Build a documented estimate of WhatsApp Business Platform charges from current official Meta rates and actual account assumptions; keep provider fees separate.
version: 1.0.0
---

# WhatsApp Business Platform Cost Model

## Purpose

Create a reviewable planning estimate for one recipient market and billing currency. Never supply guessed or stale rates as facts.

## Required inputs

- Recipient market, billing currency, and estimate period.
- Official Meta rate source and access date.
- Delivered-message volume by category and pricing tier.
- Applicable no-charge delivered quantity, with its eligibility source and calculation.
- Provider charges and tax treatment from current contracts or qualified sources.
- Estimate owner, reviewer, and decision to be supported.

## Procedure

1. Open the current official [WhatsApp Business Platform pricing page](https://whatsappbusiness.com/products/platform-pricing/) and follow the rate-card links. Record market, currency, category, tier, rate unit, effective date if shown, retrieval date, and URL.
2. Confirm the applicable recipient-market/category mapping and whether the rate is per delivered message. Split the estimate into separate lines whenever the market, category, currency, or tier differs.
3. Use a delivered-volume forecast. If the source data is sent volume, label it as a proxy and do not present it as billable volume without a defensible delivery estimate.
4. Identify no-charge cases from current official rules and actual eligible events. Record the rule, event window, and calculation; otherwise enter zero.
5. Calculate each line: `max(delivered − eligible no-charge, 0) × entered rate`. For tiers, split quantity across tiers and enter each rate separately. Confirm whether tier thresholds apply to incremental units or another basis before calculating.
6. Add provider and tax amounts as separate documented lines. Keep FX conversion and rounding assumptions visible.
7. Review arithmetic, units, dates, category mapping, duplicate volumes, fee exclusions, and eligibility with the account owner/provider. Compare the estimate with a reconciled invoice after the billing period.

## Output contract

Show the source and date, market, currency, category/tier, volume, excluded volume, billable volume, unit rate, line estimate, Meta subtotal, provider subtotal, user-confirmed taxable base and rate, estimated total, exclusions, reviewer, and open questions.

## Guardrails

- Do not reuse rates copied from a BSP article, prior invoice, or previous estimate as current Meta rates without checking the current official rate card.
- Do not hardcode free quotas, service windows, click-to-message windows, category rules, tier thresholds, or currency rates.
- Do not mix Meta charges with provider fees or taxes under one unlabeled rate.
- Do not call an estimate a quote, bill, invoice, guaranteed saving, or compliance determination.
- Do not store phone numbers, message content, or customer-level personal data in the worksheet or calculator.

