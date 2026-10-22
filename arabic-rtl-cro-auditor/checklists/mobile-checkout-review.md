# Mobile Checkout Review — {{STORE_NAME}}

Use this checklist to document a real Arabic or mixed-language checkout journey. It is not a conversion score. Mark each row **Observed**, **Not observed**, or **Not applicable**; every observation needs a screenshot, URL/state, or reproducible step. Keep the observation, possible explanation, and proposed change separate.

**Market:** ___ | **Platform:** ___ | **Device / browser:** ___ | **Language(s):** ___<br>
**Payment methods enabled for this store:** ___ | **Review date:** ___<br>
**Flow states captured:** cart ___ / customer details ___ / delivery ___ / payment ___ / confirmation ___ / error or recovery ___

## 1. RTL and visual rendering

| Check | Status | Evidence / location | Observation (fact only) |
|---|---|---|---|
| Page direction and mirrored layout are consistent | | | |
| Arabic text mixed with Latin names, codes, phone numbers, and prices reads in the intended order | | | |
| Labels, totals, errors, and buttons are not clipped, overlapped, or hidden by the keyboard | | | |
| Icons, arrows, progress indicators, and back actions communicate the actual direction | | | |
| Text remains usable at the device's normal text size and when zoomed | | | |

## 2. Forms, keyboard, and validation

| Check | Status | Evidence / location | Observation (fact only) |
|---|---|---|---|
| Each field has a persistent, understandable label | | | |
| Required and optional fields are distinguishable | | | |
| The phone field opens an appropriate telephone keyboard; numeric fields request numeric input where supported | | | |
| Address fields and examples fit the selected market's real delivery workflow | | | |
| Validation identifies the field and a clear next action in the flow language | | | |
| Entered data is preserved when a correctable error occurs | | | |

## 3. Price, delivery, and policies

| Check | Status | Evidence / location | Observation (fact only) |
|---|---|---|---|
| Currency and price basis are clear wherever a price is shown | | | |
| Delivery fees, taxes, discounts, and other charges are explained at the point required by the store's approved policy and local rules | | | |
| The customer can review the payable total before committing to payment | | | |
| Delivery timing and serviceability are stated consistently with the store's approved information | | | |
| Return, refund, and cancellation terms are reachable before purchase completion | | | |

Do not assume one tax-display pattern or delivery promise applies across markets. Verify the actual storefront policy and current local requirements with the responsible owner.

## 4. Payment and recovery

| Check | Status | Evidence / location | Observation (fact only) |
|---|---|---|---|
| Only payment methods actually enabled for this store are presented | | | |
| Method names, eligibility notes, and any installments or fees match approved provider terms | | | |
| Declined, cancelled, or pending payments explain what happened and a safe next action | | | |
| A retry or alternate method does not create a duplicate order or charge | | | |
| COD instructions, where offered, match the store's actual confirmation and collection process | | | |
| OTP, bank, fraud, and payment-provider safeguards remain intact | | | |

## 5. Access, trust, and journey continuity

| Check | Status | Evidence / location | Observation (fact only) |
|---|---|---|---|
| Guest purchase or account creation behavior is accurately documented | | | |
| Any account requirement is explained before the customer reaches a dead end | | | |
| Contact and support routes work in the selected language and market | | | |
| Progress and back-navigation preserve valid entries and explain the current step | | | |
| Pop-ups or cross-sells do not obscure required checkout actions | | | |

## 6. Measurement and evidence

| Item | Definition / source | Owner / status |
|---|---|---|
| Checkout started | Exact platform event or report; avoid collecting unnecessary personal data | |
| Payment attempt / error | Actual event names available in the implementation | |
| Completed order | System of record, deduplication key, and treatment of cancellation/return | |
| Market, device, language, and payment-method breakdown | Aggregated, privacy-appropriate dimensions available to the team | |
| Screenshot and reproducible steps | Store securely under the team's access rules | |

## Findings and next actions

For each issue, write three separate entries:

- **Observation:** What is directly visible or reproducible? Attach the evidence reference.
- **Hypothesis:** What user or system mechanism might explain it? Mark this as unverified.
- **Proposed action:** What change could address it, what could it break, and what owner must review it?

| Priority | Evidence-backed issue | Risk if changed | Effort / owner | Validation method and decision date |
|---|---|---|---|---|
| | | | | |
| | | | | |
| | | | | |

Do not rank by an invented score or promise a conversion lift. Choose a validation method that fits the change and available traffic; document the comparison period, seasonality, concurrent campaigns, and uncertainty before interpreting a before/after result.

**Scope note:** This is a review of the supplied journey and evidence. It does not certify legal compliance, payment security, provider reliability, or conversion impact. Do not bypass authentication, OTP, fraud checks, or payment controls.
