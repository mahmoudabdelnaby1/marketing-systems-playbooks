# Test eligibility and design choice

Use this before selecting a test method. It is a decision aid, not a statistical power calculator or a platform eligibility checker.

## 1. State the question precisely

Complete: “For **[population]**, does **[specific marketing intervention]**, compared with **[comparison condition]**, change **[one primary business outcome]** during **[defined window]**?” Name the system of record and the outcome date rule (for example, order date or collected-order date).

## 2. Keep three kinds of evidence separate

| Evidence | What it can support | What it cannot establish by itself |
|---|---|---|
| Attribution | Credit under a stated platform or analytics model | That the activity caused the credited outcome |
| Observational association | A relationship in observed data, subject to measured and unmeasured differences | A causal effect without additional assumptions and design |
| Controlled experiment | A causal estimate for the assigned units when assignment, exposure, measurement, and analysis remain valid | A universal result for other populations, channels, periods, or budgets |

## 3. Feasibility questions

Record evidence for each item; unknown is not a pass.

1. **Outcome integrity:** Can the primary outcome be measured consistently for both groups, including cancellations, returns, COD collection, and delays where relevant?
2. **Assignment:** What is the assignment unit (person, account, geography, campaign, or another unit), and can assignment be implemented as declared?
3. **Comparison:** Is there a credible control or comparison condition that does not create unacceptable customer or business harm?
4. **Exposure separation:** Can other campaigns, national targeting, cross-device behavior, creators, or sales channels contaminate the comparison?
5. **Data readiness:** Are historical outcome volume and variability available to assess whether the test is decision-useful? Do not invent a sample-size threshold.
6. **Timing:** Do Ramadan/Eid, White Friday, national events, payday cycles, school calendars, stock availability, delivery constraints, or planned promotions affect the window?
7. **Decision value:** Is there a named decision owner, a decision that could change, and a minimum worthwhile effect selected as a business decision?
8. **Platform fit:** If a platform-managed experiment is proposed, is the feature available to this account and objective now? Verify eligibility and setup in that platform’s current official documentation.

## 4. Choose and label the design

- **Platform-managed randomized holdout:** Use only when the platform confirms current availability and the test setup matches the question. Record who is eligible for treatment/control and which outcomes are reported.
- **Randomized geographic design:** Use when units can be assigned appropriately and campaigns, fulfillment, and other demand drivers can be separated enough to limit spillover. Review pre-period comparability and delivery constraints.
- **Other randomized design:** State assignment, enforcement, analysis, and any deviations explicitly.
- **Quasi-experimental or observational analysis:** Use only with a named method and documented assumptions, diagnostics, and limitations. Label it accurately; do not call it randomized or claim the same evidential strength.

Google’s documentation describes account-dependent availability and design considerations for its geography-based Conversion Lift. Meridian GeoX documents several geo-experiment types. These are examples of methods, not blanket recommendations or guarantees of eligibility. Re-check the official references in the README at design time.

## 5. Decision outcomes

- **Proceed to preregistration:** The outcome, assignment, comparison, contamination controls, measurement, duration, and decision use are sufficiently specified; obtain relevant approvals before launch.
- **Redesign:** A named design problem can be corrected (for example, assignment cannot be enforced or the comparison is exposed to the same activity).
- **Collect evidence first:** A material input is unknown, such as outcome completeness, variance, platform availability, or delivery lag. Name the source and period needed.
- **Do not run this test:** Expected harm, infeasible separation, or lack of a decision that could change outweighs the value of the test.

Do not treat a result as eligible merely because an ad platform displays a metric or the team has a large budget. If a statistical power analysis is needed, involve a qualified analyst and preserve the assumptions and code used.
