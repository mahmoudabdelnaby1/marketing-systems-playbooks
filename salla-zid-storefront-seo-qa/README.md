# Salla & Zid Storefront SEO Review

A platform-specific workflow for reviewing the native search fields on Salla and Zid storefront pages. It turns verified product, category, brand, homepage, blog, and additional-page facts into a documented QA queue. It does not promise rankings, generate benchmark copy, change URLs, edit robots rules, or inject structured data.

## Who it is for

Store owners and marketing teams who manage Arabic, English, or multilingual catalogues on Salla or Zid and need a repeatable way to find incomplete, inaccurate, duplicated, or stale search metadata.

## Use it when

- A store has products or categories with missing or duplicated search titles and descriptions.
- A team is preparing new products, categories, or editorial pages for publication.
- A page URL, product detail, price, availability, or language has changed and the search result needs review.
- Search Console data or a store report points to a page that deserves investigation.

## Inputs

1. Store platform, admin UI version, active language(s), market, and the page types in scope.
2. Canonical live URLs and the current visible product/category/page facts.
3. Approved brand, product, price, availability, shipping, returns, and claims data, with source and date.
4. Current platform help documents and Search Console evidence where available.
5. Change owner, reviewer, and rollback route for any URL or visibility change.

## Workflow

1. **Set a bounded scope.** Choose a representative page set and record the reason each URL is included. Do not bulk-edit an entire catalogue without a reviewed sample and rollback plan.
2. **Record the current state.** Capture the live URL, language, page title, visible heading, search title/description fields, publication and availability state, and the date checked.
3. **Check the page, not just the field.** Confirm that the page is publicly accessible, has the intended language, shows accurate information, and serves a distinct user need.
4. **Review metadata for fidelity.** Use accurate page-specific wording that reflects the visible page. Remove unsupported offers, delivery promises, location claims, and repeated keyword strings.
5. **Treat URLs as controlled changes.** Keep established URLs unless a documented migration case exists. Before a URL change, map old-to-new URLs, confirm platform behavior and redirects, review internal links, and get explicit owner approval.
6. **Make a small reviewed change.** Save one representative item or a small batch, then check the public render, language, internal links, and expected URL before continuing.
7. **Review discovery evidence.** Use Search Console coverage, indexing, impressions, clicks, and query/page reports as observations; distinguish crawl/index status from ranking or business outcomes.
8. **Close with a change log.** Record changed fields, reviewer, date, source references, observed result, unresolved issues, and rollback details.

## Platform field map

| Page type | Salla (verify current dashboard) | Zid (verify current dashboard) | Review focus |
|---|---|---|---|
| Homepage | Marketing → Search Engine Optimization → general/homepage settings (help path may evolve) | SEO store settings for home page (help path may evolve) | Brand, proposition, language, and visible homepage content match. |
| Product | Product detail → SEO enhancements | SEO products | Product facts, variants, identifiers when appropriate, price/availability accuracy, and unique page intent. |
| Category | Products → Categories & Options → category SEO enhancements | SEO category | Category membership and page content match; no invented range, stock, or delivery claims. |
| Brand | Salla supports brand SEO fields in its current guide | Verify current Zid support and account UI | Use only where the brand page is a meaningful public destination. |
| Blog / additional pages | Salla blog and its SEO fields | SEO for additional pages; blog/page support can depend on theme or dashboard version | Index only useful, complete pages with clear ownership and language. |

Paths and features can change. If the live dashboard differs from the linked help article, record the difference and follow the current official UI; do not guess or apply a bulk edit.

## Deliverables

- A prioritized page-level issue register with evidence, owner, and proposed action.
- A short sample of revised metadata for human approval.
- A change log and post-save QA record.
- A list of URLs and platform/source questions needing escalation.

## Search and AI visibility boundaries

This workflow improves the completeness and accuracy of native store content; it cannot guarantee crawl, indexing, rankings, rich results, AI citations, or sales. Search features can rewrite titles and snippets. Useful, original, visible content and sound technical access remain central. Structured data must reflect visible page content and platform support; this toolkit does not generate injectable markup. `llms.txt`, keyword repetition, fixed word counts, and FAQ markup are not treated as ranking shortcuts.

## Source references

- [Salla: Improve your store visibility on search engines](https://help.salla.sa/en/article/improve-your-store-visibility-on-search-engines-seo/oi134aj2ud6ts12ysumrm5za)
- [Zid: SEO for the store homepage and products/categories](https://help.zid.sa/seo-store/)
- [Zid: SEO for additional pages](https://help.zid.sa/seo-additional-pages/)
- [Google Search: Generative AI features guidance](https://developers.google.com/search/docs/fundamentals/ai-optimization-guide)
- [Google Search: Structured data policies](https://developers.google.com/search/docs/appearance/structured-data/sd-policies)

Recheck the platform help articles before following dashboard paths; their UI and feature availability can change.
