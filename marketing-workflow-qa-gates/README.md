# Marketing Workflow QA & Evidence Gates

Use these review gates to connect campaign, content, commerce, measurement and customer operations before launch—and to record what was actually verified.

## Use it when

Several teams or channels contribute to one customer journey, and a checklist tied to evidence and owners is needed before a change goes live.

## Prepare

Decision and owner; audience, offer and markets; channel/asset versions; destination pages; consent and data flows; event definitions; operational handoffs; source links and change dates.

## Workflow

1. Decision and claims: state the intended decision, evidence, assumptions and review owner. Separate a hypothesis from a measured result.
2. Campaign and links: align objective, audience, offer, budget assumptions, landing page and tagged URLs; check redirects and market/language parity.
3. Creative and content: confirm factual claims, rights, version approval, platform fit, accessibility and destination consistency.
4. Experience and commerce: complete the main mobile journey, validation, price/promotion, stock, checkout and recovery paths with real test cases.
5. Measurement and privacy: map browser/server events, consent, identifiers, deduplication and order/CRM outcomes; record which platform diagnostics and backend records were checked.
6. Lifecycle and operations: verify opt-in, suppression, frequency, routing, ownership and escalation for email, messaging and automation.
7. Search and discovery: check visible page facts, metadata, language routing, canonical/hreflang and crawler rules without changing established URLs or bot access casually.
8. Launch and learning: record owner, timestamp, evidence link, unresolved risk, rollback/stop condition and post-launch check. Close only the items with recorded evidence.

## Included

A cross-functional review register with decision, owner, evidence, state, risk and follow-up fields; plus eight gates for campaign, creative, commerce, measurement, lifecycle and discovery work. It complements specialist playbooks and does not replace platform, legal, privacy or engineering review.

## Review boundaries

A checked box is not proof by itself. Attach a dated source, screenshot, test record or system output and state its limits. Do not claim launch success, compliance or production readiness from a static checklist.

## Official and primary references

- This cross-functional checklist points to specialist toolkit documents linked from the repository index.


## Cross-tool integration gates

These additions condense recurring, useful patterns from the reviewed material into reusable checks. Use the specialist toolkit named in each section for detailed setup. The gates below are planning and QA prompts, not proof that a campaign or system passed.

### 01 · Measurement, attribution & consent

Define events and outcome fields before implementation. Check consent behavior, event identity and deduplication, offline/CRM handoffs, reconciliation to orders, and the uncertainty in experiment or modeled estimates.

Related toolkits: [`commerce-measurement-planning`](../commerce-measurement-planning/README.md), [`revenue-roas-reconciliation`](../revenue-roas-reconciliation/README.md), [`mena-incrementality-test-designer`](../mena-incrementality-test-designer/README.md).

### 02 · Search & AI discovery

Record query, market, language, date and visible answer/citation. Check crawl access, canonical and language routes, page facts and schema parity; treat AI visibility as an observation, not a ranking promise.

Related toolkits: [`arabic-aeo-geo-visibility-kit`](../arabic-aeo-geo-visibility-kit/README.md), [`salla-zid-storefront-seo-qa`](../salla-zid-storefront-seo-qa/README.md).

### 03 · Campaign operations & governance

Align audience, objective, offer, landing page, budget assumptions, campaign URL and owner. Keep a dated change log, claim evidence, approval state, access dependency and stop condition.

Related toolkits: [`mena-cross-border-ppc-guardrails`](../mena-cross-border-ppc-guardrails/README.md), [`mena-ad-compliance-precheck`](../mena-ad-compliance-precheck/README.md), [`bilingual-client-reporting-workflow`](../bilingual-client-reporting-workflow/README.md).

### 04 · Creative, content & rights

Approve the factual claim, asset version, usage rights, audience fit, language, CTA and destination together. Treat public competitor examples as creative observations, not proof of performance.

Related toolkits: [`organic-content-video-operations`](../organic-content-video-operations/README.md), [`tiktok-spark-ugc-mena-factory`](../tiktok-spark-ugc-mena-factory/README.md).

### 05 · Commerce, feeds & conversion

Reconcile product facts and catalog items with the store. Check stock, price, promotion terms, mobile product-to-checkout flow, delivery/return paths and settled order outcomes.

Related toolkits: [`ecommerce-funnel-diagnostic`](../ecommerce-funnel-diagnostic/README.md), [`ecommerce-unit-economics`](../ecommerce-unit-economics/README.md), [`arabic-gmc-feed-architect`](../arabic-gmc-feed-architect/README.md).

### 06 · Arabic localization & parity

Maintain a verified fact source and compare the same promise, offer, CTA, URL and event across Arabic and English. Include local-market review and real RTL/mixed-script tests.

Related toolkits: [`arabic-market-copy-localizer`](../arabic-market-copy-localizer/README.md), [`arabic-rtl-cro-auditor`](../arabic-rtl-cro-auditor/README.md).

### 07 · Email, lifecycle & automation

Check lawful/permission basis, suppression, frequency, provider authentication, event trigger, customer context, routing, ownership and human escalation before a message flow is enabled.

Related toolkits: [`permission-email-deliverability-review`](../permission-email-deliverability-review/README.md), [`salla-zid-klaviyo-retention-architect`](../salla-zid-klaviyo-retention-architect/README.md), [`whatsapp-order-follow-up`](../whatsapp-order-follow-up/README.md).

### 08 · Journey, landing page & CRO

Begin with the customer task and observed friction. Set one hypothesis and primary metric, test the full mobile path, verify performance and validation, and avoid treating an underpowered test as a winner.

Related toolkits: [`ecommerce-funnel-diagnostic`](../ecommerce-funnel-diagnostic/README.md), [`arabic-rtl-cro-auditor`](../arabic-rtl-cro-auditor/README.md).

### 09 · Integrations & technical operations

Verify the current provider/API contract, account access, field mapping, failure behavior, retry/idempotency and data minimization. Name the owner for monitoring and recovery; do not publish demo integrations as production-ready.

Related toolkits: [`commerce-measurement-planning`](../commerce-measurement-planning/README.md), [`salla-zid-klaviyo-retention-architect`](../salla-zid-klaviyo-retention-architect/README.md).

### 10 · Reporting & evidence governance

Define each metric and source before reporting. Preserve date range and attribution window, distinguish platform-attributed, modeled and observed business outcomes, and link every claim to dated evidence.

Related toolkits: [`bilingual-client-reporting-workflow`](../bilingual-client-reporting-workflow/README.md), [`revenue-roas-reconciliation`](../revenue-roas-reconciliation/README.md).
