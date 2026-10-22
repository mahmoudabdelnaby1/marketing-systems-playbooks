# Marketing Incrementality Test Design

A practical framework for deciding whether a marketing question can be answered with a controlled experiment, choosing a feasible design, documenting it before launch, and interpreting the result within its evidence limits. It is designed for teams working across MENA and other markets; it does not assume that a platform feature, data volume, or market split is available.

## The decision this guide supports

Use this toolkit when a team needs to distinguish attributed activity from evidence that a campaign caused additional business outcomes. The output may be **proceed with a controlled test**, **redesign**, or **collect more evidence first**. “Not yet” is a valid decision.

## Workflow

1. Define one business decision, target population, intervention, primary outcome, and system of record.
2. Check data quality, design feasibility, risk, seasonality, outcome delay, and whether treatment and comparison can remain meaningfully distinct.
3. Select a design appropriate to the question: a platform-managed randomized holdout, a randomized geographic test, or another controlled design supported by the available method. If randomization is not feasible, label the work observational or quasi-experimental and state its assumptions; do not describe it as randomized evidence.
4. Record the hypothesis, units, outcome, analysis, duration, stop rules, and decision thresholds before launch.
5. Log material events during the test, analyze at the declared end, compare with the pre-agreed decision rule, and archive positive, null, negative, and inconclusive results.

## Files

- framework/test-eligibility.md — evidence and feasibility decision path.
- templates/preregistration.md — the pre-launch design record.
- templates/confounder-register.md — market, delivery, and business events to monitor.
- templates/results-interpretation.md — a bounded readout template.
- tests/design-review-cases.md — review scenarios for common design and reporting failures.

## Important boundaries

Attribution reports how a chosen model assigns credit; it does not by itself establish causation. A before/after comparison can be useful operational evidence, but it is not automatically a controlled experiment. An experiment’s conclusion applies to the tested population, intervention, outcome definition, and time window. This toolkit does not calculate statistical power, replace a statistician, operate an ad platform, or guarantee a lift. Confirm platform availability and mechanics in current official documentation before committing to a design.

## Starting references

- Google Ads Help, [Conversion Lift based on geography](https://support.google.com/google-ads/answer/14102986?hl=en).
- Google Meridian, [GeoX types of experiments](https://developers.google.com/meridian/geox/types-of-experiments).
- Google Ads Help, [About custom experiments](https://support.google.com/google-ads/answer/10683687?hl=en).

Platform features and requirements change. Record the official source and access date used for each design; do not copy thresholds from an old project or template.

## Arabic summary

إطار عملي لتحديد ما إذا كان سؤال التسويق يمكن اختباره بتجربة مقارنة مناسبة، واختيار تصميم قابل للتنفيذ، وتوثيقه قبل الإطلاق، ثم قراءة النتيجة ضمن حدود الأدلة. قد تكون النتيجة: **ابدأ اختبارًا مضبوطًا** أو **أعد تصميمه** أو **اجمع أدلة إضافية أولًا**. لا يفترض الدليل توافر ميزة معينة أو حجم بيانات أو تقسيم جغرافي مناسب.

يفصل الإطار بين الإسناد والارتباط والزيادة التي يمكن نسبتها سببيًا إلى النشاط. المقارنة قبل/بعد ليست تلقائيًا تجربة مضبوطة، وأي نتيجة تظل مرتبطة بالجمهور والتدخل والنتيجة والمدة التي اختُبرت. تحقّق من وثائق المنصة الرسمية الحالية قبل اعتماد أي متطلبات أو إعدادات.
