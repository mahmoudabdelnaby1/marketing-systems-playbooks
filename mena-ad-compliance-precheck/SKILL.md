---
name: mena-ad-compliance-precheck
description: "Helps review advertising claims, creator briefs, and campaign assets for Saudi Arabia, the UAE, and Egypt. Prompts users to identify product scope, substantiation, current primary sources, and issues requiring regulator or legal review. Use as a human-in-the-loop checklist, not as legal advice or an approval decision."
---

# MENA Advertising Pre-Flight Review

## Purpose

Support a documented, human-led pre-flight review. Identify missing evidence and questions; do not make legal determinations, assert a permit is required, or promise an ad will be approved.

> Verify current requirements with the responsible regulator or qualified local counsel. The SFDA source linked here is specifically about medical devices; do not generalize it to all health advertising.

## Workflow

1. **Define scope:** record the product/service, market, advertiser, creator, channel, and intended audience. If classification is uncertain, stop and ask for qualified review.
2. **Collect evidence:** list each factual, efficacy, comparative, pricing, availability, and testimonial claim alongside its evidence and owner. Mark unsupported claims for review; do not invent a rewrite that changes the facts.
3. **Check applicable requirements:** use current primary sources for the exact product and activity. An approval to sell a product does not, by itself, establish approval for a specific advertisement. Distinguish platform policy from local law.
4. **Check creator and data use:** record disclosure and licensing questions for confirmation. For personal data, document purpose, lawful basis/consent where applicable, minimization, access, and retention. Do not collect sensitive data unless necessary and appropriately authorized.
5. **Record decision:** identify evidence reviewed, official sources and dates checked, reviewer, unresolved questions, and the person responsible for final approval. A human with appropriate authority makes the decision.

## Output format

| Asset / claim | Evidence supplied | Source checked and date | Question or risk to resolve | Owner / status |
|---|---|---|---|---|

## Boundaries

- Phrase flags in `datasets/claim-review-lexicon-ar-en.json` are prompts for human review, not automatic bans or legal conclusions.
- Do not quote old fee, approval-time, age, comment, discount, or permit statements from archived drafts unless independently verified against a current primary source and its exact scope.
- This workflow is not legal advice, regulator approval, or a substitute for qualified local counsel.

