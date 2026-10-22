# Arabic Negative Keyword Review

A controlled workflow for identifying irrelevant paid-search queries and reviewing Arabic spelling and morphology before changing account exclusions.

## Workflow

1. Export actual search terms from the intended account, campaign, date range, and market. Preserve the source export and note filters.
2. Label each term by intent and business relevance. Separate clearly irrelevant intent from uncertain terms that need human review.
3. Generate candidate Arabic variants for review, including attached articles and prepositions, spelling variants, singular/plural forms, and dialect wording. Treat these as candidates; do not automatically exclude them.
4. Check Google’s current negative-keyword matching behavior. Negative keywords do not automatically cover close variants in the same way positive keywords can, so review actual query variants and the chosen match type in the account.
5. Check the proposed exclusions against converting or valuable queries, brand terms, product names, and campaign scope. Prefer the narrowest appropriate scope.
6. Record owner approval, date, reason, match type, and destination campaign before applying changes.
7. Monitor search terms, spend, qualified outcomes, and unintended traffic loss after the change. Keep a rollback copy.

## Language and network check

Before separating or combining campaigns by language, confirm the campaign type and network. As of Google's September 2026 change, manual campaign-level language targeting is removed for Search campaigns and no longer applies to the Search portion of Performance Max; ads on Search are matched using ad language and Google's language signals. Language settings continue to apply to eligible non-Search Performance Max channels. Verify the current help page and the live account before changing structure.

## Candidate log

| Search term | Intent label | Candidate negative | Match type | Scope | Evidence / risk | Reviewer decision |
| --- | --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |  |

## Boundaries

This is not a prebuilt negative list or a guarantee against wasted spend. Do not paste generic lists into an account without checking the offer and actual search terms. Match behavior and controls can change; verify current Google Ads documentation and the live account before editing.

## Official reference

- [Google Ads: About negative keywords](https://support.google.com/google-ads/answer/2453972?hl=en)
- [Google Ads: About language targeting](https://support.google.com/google-ads/answer/1722078?hl=en-GB)
