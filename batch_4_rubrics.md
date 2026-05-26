# Batch 4 Evaluation Artifacts

Evaluation artifacts for the 16 runnable tasks in `manual_deep_research_batch_004.md`.

Phase 10 rule:
- Core tasks use a task-level rubric with five fixed criteria: Coverage, Accuracy, Reasoning, Use of evidence, Clarity and structure.
- Each Core criterion is scored 0-2, for 10 total points.
- Set tasks use a gold set, not a narrative rubric. Set scoring is precision, recall, and F1 against the bounded gold set.

---

## 1. CORE-ECON-17

rubric_id: CORE-RUBRIC-B04-CORE-ECON-17
task_type: Core
research_object: Microsoft shareholder distributions
answer_unit: quarterly dividend per share amount in fiscal 2024

### Key Facts From Source Bundle

- Fiscal-year 2024 dividend rows show a per-share dividend amount of **$0.75**.
- The answer unit is the quarterly dividend per share, not annualized dividend or annual total.
- Dividend declaration, record date, and payment date are distinct from the dividend amount.
- Fiscal-year 2024 rows must not be mixed with later calendar-year dividend increases.
- The official annual report or dividend table is controlling.

### Expected Response Sections

- Conclusion with the fiscal 2024 quarterly dividend per-share amount.
- Source comparison anchored in the official annual report/dividend table.
- Boundary explanation about quarterly versus annualized amount and fiscal versus calendar year.
- Caveat about declared/paid/record-date treatment or later dividend changes.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes amount, fiscal-year boundary, quarterly boundary, evidence, caveat, and confidence.
- 1: Gives the amount but omits an important boundary or evidence section.
- 0: Does not answer the quarterly dividend question.

**Accuracy**
- 2: Reports **$0.75 per share** for fiscal 2024 quarterly dividend rows.
- 1: Gives $0.75 but with unclear quarterly/fiscal-year wording.
- 0: Reports annual total, later dividend increase, or a date instead of the value.

**Reasoning**
- 2: Separates quarterly amount from annualized amount, and declared/paid/record dates from value.
- 1: Mentions one distinction but leaves another unclear.
- 0: Conflates dividend amount with payment/record date or annual total.

**Use of Evidence**
- 2: Uses the official annual report or dividend table as anchor and corroborates only consistency/update status.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported market snippets or later dividend notices as the 2024 answer.

**Clarity and Structure**
- 2: Concise answer with conclusion, comparison, caveat, and confidence.
- 1: Understandable but missing one expected section.
- 0: Unclear or mostly unrelated to fiscal 2024 dividends.

### Common Failure Modes

- Reporting the annual total instead of quarterly amount.
- Mixing fiscal-year and calendar-year rows.
- Treating record date or payment date as the dividend value.
- Using a later dividend increase as the 2024 answer.

### Borderline Cases

- Accept "75 cents per share" as equivalent.
- A response can mention annual total only if the quarterly $0.75 answer remains primary.
- Later dividend changes should be caveated, not substituted.

---

## 2. CORE-ECON-06

rubric_id: CORE-RUBRIC-B04-CORE-ECON-06
task_type: Core
research_object: Citigroup share repurchase authorization
answer_unit: $20 billion multiyear common stock repurchase programme and $1.5 billion planned first-quarter repurchases

### Key Facts From Source Bundle

- On **13 January 2025**, the board authorised a new **$20 billion** multiyear common stock repurchase programme.
- Planned first-quarter 2025 repurchases were **$1.5 billion**.
- Board authorisation is distinct from executed buybacks.
- The multiyear programme amount is distinct from the quarter-specific planned amount.
- The figures concern common stock repurchases, not dividends or total capital return.

### Expected Response Sections

- Conclusion with the authorisation date, $20 billion programme, and $1.5 billion planned Q1 repurchases.
- Source comparison anchored in official company/bank reporting.
- Boundary explanation about authorisation, planned repurchases, executed buybacks, and multiyear versus quarterly amounts.
- Caveat about plans versus completed repurchases.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Covers date, both amounts, programme/quarter boundary, evidence, caveat, and confidence.
- 1: Gives both amounts but omits date or boundary detail.
- 0: Omits the programme or planned-quarter component.

**Accuracy**
- 2: Reports **13 January 2025**, **$20 billion** multiyear programme, and **$1.5 billion** planned Q1 2025 repurchases.
- 1: Gets two components correct or gives one with minor ambiguity.
- 0: Reports $1.5 billion as total programme size or treats the programme as fully executed.

**Reasoning**
- 2: Distinguishes authorisation, planned repurchases, executed buybacks, remaining authorisation, and timing.
- 1: Mentions authorisation/planning but not all amount boundaries.
- 0: Conflates planned and executed repurchases or repurchases and dividends.

**Use of Evidence**
- 2: Anchors in official company reporting and checks compatible later execution/update data.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported financial-news snippets or total capital-return figures only.

**Clarity and Structure**
- 2: Clearly separates the multiyear programme from Q1 planned repurchases.
- 1: Mostly clear but somewhat compressed or incomplete.
- 0: Confusing capital-return summary.

### Common Failure Modes

- Reporting $1.5 billion as the total programme size.
- Treating the authorisation as already fully executed.
- Omitting the January 2025 timing.
- Confusing repurchases with dividends or capital distributions generally.

### Borderline Cases

- Accept "share buyback" for "repurchase" if common stock is clear.
- If actual Q1 buybacks are later known, they should be reported as an update, not the planned amount.
- Do not require detailed board minutes if official reporting supports the authorisation.

---

## 3. BND-CORE-PAIR-015

rubric_id: CORE-RUBRIC-B04-BND-CORE-PAIR-015
task_type: Core
research_object: Nestle advertising and marketing spend
answer_unit: 8.1% of sales in 2024 and 9% target by end-2025

### Key Facts From Source Bundle

- Advertising and marketing spend recovered to **8.1% of sales in 2024**.
- Management planned to increase it to **9% by the end of 2025**.
- The measure is percentage of sales, not absolute spend.
- The 2024 value is actual/reported; the 2025 value is a target/plan.
- Later reports may revise or supersede the target.

### Expected Response Sections

- Conclusion with the 2024 actual and end-2025 target.
- Source comparison anchored in official company review/reporting.
- Boundary explanation separating actuals from management plans and percent-of-sales from absolute spend.
- Caveat about later reports or target status.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes both figures, timing, percent-of-sales boundary, evidence, caveat, and confidence.
- 1: Includes both figures but omits target/actual distinction or caveat.
- 0: Omits one of the two key figures.

**Accuracy**
- 2: Reports **8.1% of sales in 2024** and **9% target by end-2025**.
- 1: Gives both percentages but with unclear timing/status.
- 0: Treats 9% as 2024 actual or gives absolute spend only.

**Reasoning**
- 2: Separates actual 2024 spend from 2025 target and percent-of-sales from absolute spend.
- 1: Mentions status but leaves measurement boundary unclear.
- 0: Conflates actual and target or measure type.

**Use of Evidence**
- 2: Uses official company reporting as anchor and corroborates update/target status.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic marketing commentary or unsupported numbers.

**Clarity and Structure**
- 2: Clear two-part answer with comparison, caveat, and confidence.
- 1: Understandable but missing one expected section.
- 0: Unclear or broad marketing strategy discussion.

### Common Failure Modes

- Treating 9% as the 2024 actual.
- Reporting absolute marketing spend instead of share of sales.
- Omitting the target timing.
- Ignoring that 2025 is a plan/target, not a completed result.

### Borderline Cases

- Accept "advertising and marketing investment" if it clearly matches the source measure.
- If later 2025 actuals exist, they should be caveated separately.
- Minor spelling variants for the company name do not affect scoring.

---

## 4. CORE-SCI-09

rubric_id: CORE-RUBRIC-B04-CORE-SCI-09
task_type: Core
research_object: Ukraine reconstruction needs estimate
answer_unit: US$486 billion, equivalent to 2.8 times estimated 2023 nominal GDP

### Key Facts From Source Bundle

- Reconstruction needs are estimated at **US$486 billion**.
- This is equivalent to **2.8 times estimated 2023 nominal GDP**.
- Needs are distinct from damages, losses, committed financing, or financing gaps.
- Estimate date and reconstruction-period scope matter.
- Later assessments may revise the amount or GDP multiple.

### Expected Response Sections

- Conclusion with the amount and GDP multiple.
- Source comparison anchored in the official reconstruction assessment/source.
- Boundary explanation separating needs, damages, losses, financing, and GDP baseline.
- Caveat about estimate date, scope, and later revisions.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes amount, GDP multiple, needs/damages boundary, evidence, caveat, and confidence.
- 1: Gives amount but omits GDP multiple or boundary detail.
- 0: Does not identify reconstruction needs.

**Accuracy**
- 2: Reports **US$486 billion** and **2.8 times estimated 2023 nominal GDP**.
- 1: Gives one component correctly or a close amount with unclear baseline.
- 0: Reports damages, losses, committed financing, or another amount as needs.

**Reasoning**
- 2: Distinguishes total needs from damages/losses/financing gaps and preserves nominal GDP baseline.
- 1: Mentions needs/damages distinction but leaves baseline unclear.
- 0: Treats the estimate as fully funded or as damage only.

**Use of Evidence**
- 2: Anchors in official assessment evidence and compares revision/date-compatible sources.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported or incompatible Ukraine aid figures.

**Clarity and Structure**
- 2: Clear amount and multiple with comparison, caveat, and confidence.
- 1: Understandable but missing one section.
- 0: Unfocused reconstruction essay.

### Common Failure Modes

- Reporting damages instead of reconstruction needs.
- Omitting the GDP multiple.
- Treating the estimate as a fully funded amount.
- Mixing nominal GDP baseline with real GDP or later GDP estimates.

### Borderline Cases

- Accept "USD" and "US$" as equivalent.
- Later RDNA-style revisions can be mentioned only if the original source-bundle estimate remains clear.
- If the answer gives the correct amount but not the GDP multiple, accuracy is partial.

---

## 5. CORE-SCI-07

rubric_id: CORE-RUBRIC-B04-CORE-SCI-07
task_type: Core
research_object: Netherlands teacher salary change
answer_unit: 25% nominal statutory salary increase between 2015 and 2023

### Key Facts From Source Bundle

- In the Netherlands, nominal statutory salaries increased by **25%** between **2015 and 2023**.
- The teacher profile is lower secondary teachers with **15 years of experience**.
- The measure is nominal, not real/inflation-adjusted.
- Statutory salary differs from actual compensation, take-home pay, or total remuneration.
- Education level, profile, and reference years must be preserved.

### Expected Response Sections

- Conclusion with the 25% nominal statutory salary increase.
- Source comparison anchored in official education indicators/source.
- Boundary explanation about nominal/real, statutory/actual compensation, teacher profile, and years.
- Caveat about comparability or salary-definition limits.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes percentage, country, years, teacher profile, evidence, caveat, and confidence.
- 1: Gives the percentage but omits profile or measure boundary.
- 0: Does not answer the salary-change question.

**Accuracy**
- 2: Reports **25% nominal statutory salary increase from 2015 to 2023** for the specified Netherlands teacher profile.
- 1: Gives 25% but with unclear profile or nominal/statutory wording.
- 0: Reports real salary growth, another country, or all-teacher compensation.

**Reasoning**
- 2: Distinguishes nominal/real, statutory/actual compensation, education level, experience profile, and reference years.
- 1: Mentions one or two boundaries but leaves key comparability unclear.
- 0: Treats the value as all teachers' pay or take-home compensation.

**Use of Evidence**
- 2: Uses official education indicators/reporting and corroborates definition/year compatibility.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic salary reports or incompatible labour data.

**Clarity and Structure**
- 2: Concise conclusion with comparison, caveat, and confidence.
- 1: Mostly clear but incomplete.
- 0: Unclear or broad education-pay discussion.

### Common Failure Modes

- Reporting real salary growth.
- Applying the value to all teachers or all education levels.
- Omitting the 15-years-experience profile.
- Confusing statutory salaries with take-home pay or total compensation.

### Borderline Cases

- Partial credit is appropriate if the profile is missing but the measure and years are correct.
- Do not require currency amounts; the answer unit is percentage change.
- If real salary is discussed, it must be separated from the nominal statutory answer.

---

## 6. CORE-ECON-11

rubric_id: CORE-RUBRIC-B04-CORE-ECON-11
task_type: Core
research_object: OECD unemployment rate in May 2024
answer_unit: 4.9% unemployment rate in May 2024

### Key Facts From Source Bundle

- The OECD unemployment rate was **4.9% in May 2024**.
- The measure is OECD-wide/area-wide, not a single national rate.
- The reference month is May 2024.
- Seasonally adjusted versus unadjusted status matters if specified.
- Population coverage and later revisions should be caveated.

### Expected Response Sections

- Conclusion with the 4.9% May 2024 OECD unemployment rate.
- Source comparison anchored in official labour-market/OECD evidence.
- Boundary explanation about area-wide rate, reference month, adjustment, and coverage.
- Caveat about later revisions.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes rate, month, OECD scope, evidence, caveat, and confidence.
- 1: Gives rate but omits month, scope, or caveat.
- 0: Does not answer the unemployment-rate question.

**Accuracy**
- 2: Reports **4.9% in May 2024** for the OECD unemployment rate.
- 1: Gives 4.9% with unclear month/scope.
- 0: Reports a national rate or another labour-market measure.

**Reasoning**
- 2: Distinguishes OECD-wide rate, national rates, adjustment status, reference month, and population coverage.
- 1: Mentions scope or month but not both clearly.
- 0: Confuses unemployment with employment or labour-force measures.

**Use of Evidence**
- 2: Anchors in official labour-market data and checks compatible updates/revisions.
- 1: Uses one relevant source with limited comparison.
- 0: Uses incompatible national data or unsupported values.

**Clarity and Structure**
- 2: Clear numeric conclusion with comparison, caveat, and confidence.
- 1: Understandable but missing a section.
- 0: Unclear labour-market discussion.

### Common Failure Modes

- Reporting a single country's unemployment rate.
- Using a later month without noting the update.
- Confusing unemployment rate with employment rate.
- Omitting the OECD coverage boundary.

### Borderline Cases

- This overlaps with Batch 2's unemployment item; score consistently.
- "Around 4.9%" is acceptable if source scope and month are clear.
- Later revised values should be caveated against the May 2024 source context.

---

## 7. CORE-POL-06

rubric_id: CORE-RUBRIC-B04-CORE-POL-06
task_type: Core
research_object: EU digital-services residual error rate control metric
answer_unit: target below 2% and estimated 2024 result of 0.5%

### Key Facts From Source Bundle

- The residual error-rate target is **below 2%**.
- The estimated 2024 result is **0.5%**.
- Target threshold and estimated result are different.
- Residual error differs from gross error.
- The metric concerns payments, controls, or audit findings according to the source, not service quality generally.

### Expected Response Sections

- Conclusion with target and estimated 2024 result.
- Source comparison anchored in official activity/control reporting.
- Boundary explanation about target versus result, residual versus gross error, and reporting scope.
- Caveat about estimated status and audit/control context.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes both values, reporting year, metric scope, evidence, caveat, and confidence.
- 1: Gives both values but omits estimated/status or residual/gross boundary.
- 0: Omits target or result.

**Accuracy**
- 2: Reports target **below 2%** and estimated 2024 result **0.5%**.
- 1: Gives one correct value and one ambiguous value.
- 0: Reports 2% as result or confuses the metric entirely.

**Reasoning**
- 2: Distinguishes target/result, residual/gross error, reporting year, and control/audit context.
- 1: Mentions target/result but leaves residual/gross distinction unclear.
- 0: Treats the metric as a general service-quality indicator.

**Use of Evidence**
- 2: Uses official reporting as anchor and corroborates metric definition/status.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported performance or service-quality figures.

**Clarity and Structure**
- 2: Clear two-value answer with comparison, caveat, and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing or unrelated.

### Common Failure Modes

- Reporting 2% as the result.
- Confusing residual and gross error rates.
- Omitting the estimated nature of the 2024 result.
- Treating the metric as a general service-quality indicator.

### Borderline Cases

- Accept "less than 2%" as equivalent to below 2%.
- If the answer gives 0.5% without "estimated", accuracy can still be high but caveat/reasoning should be lower.
- Do not reward broader EU audit metrics unless the residual error metric is isolated.

---

## 8. BND-CORE-PAIR-043

rubric_id: CORE-RUBRIC-B04-BND-CORE-PAIR-043
task_type: Core
research_object: EU administrative burden reduction objective
answer_unit: 25-35% administrative burden reduction objective

### Key Facts From Source Bundle

- The objective is to cut administrative burden by **at least 25-35%**.
- The 25% and 35% figures may refer to different scopes or target groups.
- The objective is political/programmatic unless adopted measures are separately identified.
- Administrative burden is narrower than broader compliance cost or budget cuts.
- Implementation and measurement remain uncertain.

### Expected Response Sections

- Conclusion with the 25-35% administrative burden reduction objective.
- Source comparison anchored in official regulatory simplification material.
- Boundary explanation about political objective, adopted measures, burden/compliance cost, and scope.
- Caveat about implementation and measurement.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes range, objective status, scope distinction, evidence, caveat, and confidence.
- 1: Gives range but omits objective/adoption or scope caveat.
- 0: Does not identify the burden-reduction objective.

**Accuracy**
- 2: Reports the **25-35%** administrative burden reduction objective with scope awareness.
- 1: Reports only 25% or 35% but indicates a broader range/scope.
- 0: Treats the figure as achieved or reports budget cuts/compliance cost without support.

**Reasoning**
- 2: Distinguishes objective from adopted measures, administrative burden from compliance cost, and 25% versus 35% scope.
- 1: Mentions one boundary but leaves scope unclear.
- 0: Conflates objective with achieved reduction or budget savings.

**Use of Evidence**
- 2: Anchors in official simplification material and corroborates scope/implementation status.
- 1: Uses one relevant source with limited comparison.
- 0: Uses political commentary without source-specific scope.

**Clarity and Structure**
- 2: Clear concise answer with comparison, caveat, and confidence.
- 1: Mostly clear but incomplete.
- 0: Unfocused regulatory-policy answer.

### Common Failure Modes

- Reporting only 25% or only 35% without scope.
- Treating the objective as achieved.
- Confusing burden reduction with budget cuts.
- Ignoring whether the figure refers to businesses, SMEs, or a narrower group.

### Borderline Cases

- If the answer says "25%, and 35% for SMEs" or equivalent scope logic, accept if source-consistent.
- Do not penalize uncertainty in the range if the caveat explains source wording.
- Later adopted measures should be separated from the original objective.

---

## 9. BND-CORE-PAIR-040

rubric_id: CORE-RUBRIC-B04-BND-CORE-PAIR-040
task_type: Core
research_object: EU artificial-intelligence regulation timing
answer_unit: entry into force on 1 August 2024 and full applicability on 2 August 2026

### Key Facts From Source Bundle

- The regulation entered into force on **1 August 2024**.
- It is fully applicable on **2 August 2026**.
- Some obligations apply on different dates.
- Entry into force is distinct from full applicability.
- Delegated or technical rules are separate from the main regulation timeline.

### Expected Response Sections

- Conclusion with both dates.
- Source comparison anchored in official legal text or official legal summary.
- Boundary explanation about entry into force, full applicability, staged exceptions, and delegated rules.
- Caveat about obligations with different dates.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes both dates, staged-applicability boundary, evidence, caveat, and confidence.
- 1: Gives both dates but omits exceptions or source comparison.
- 0: Gives only one date or does not answer timing.

**Accuracy**
- 2: Reports **1 August 2024** entry into force and **2 August 2026** full applicability.
- 1: Gives one exact date and one partial/ambiguous date.
- 0: Treats proposal/adoption dates as the regulation timeline.

**Reasoning**
- 2: Distinguishes entry into force, full applicability, exceptions, staged obligations, and delegated rules.
- 1: Mentions entry/applicability distinction but omits staged exceptions.
- 0: Treats full applicability as entry into force.

**Use of Evidence**
- 2: Uses official legal text/summary and corroborates timeline/status.
- 1: Uses one relevant source with limited comparison.
- 0: Uses proposal-era material or unsupported summaries.

**Clarity and Structure**
- 2: Clear legal/status conclusion with comparison, caveat, and confidence.
- 1: Understandable but incomplete.
- 0: Confusing or broad AI Act discussion.

### Common Failure Modes

- Giving only one date.
- Treating full applicability as entry into force.
- Ignoring staged exceptions.
- Reporting a proposal date rather than the adopted regulation's timeline.

### Borderline Cases

- If the answer names "AI Act" explicitly, that is acceptable if timing remains precise.
- Later delegated acts should not replace the main timing.
- Minor timezone/publication-date discussion should not reduce score if both legal dates are right.

---

## 10. CORE-SCI-12

rubric_id: CORE-RUBRIC-B04-CORE-SCI-12
task_type: Core
research_object: regional school water-service availability
answer_unit: close to 50% availability in Sub-Saharan Africa and at least 90% in other regions

### Key Facts From Source Bundle

- Water-related services are available in close to **50% of schools in Sub-Saharan Africa**.
- In all other regions, these services are available in **at least 90% of schools**.
- The measure is school-level water-related service availability.
- It should not be replaced by household water access, sanitation, hygiene, or electricity unless bundled by the source.
- Region grouping, service definition, data year, and measured/modelled status matter.

### Expected Response Sections

- Conclusion with both regional availability statements.
- Source comparison anchored in the education indicator source.
- Boundary explanation about region group, school-level service definition, and data status.
- Caveat about latest data year and service comparability.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes Sub-Saharan Africa figure, other-region comparison, service scope, evidence, caveat, and confidence.
- 1: Gives one figure or omits service/region boundary.
- 0: Does not answer the school water-service availability question.

**Accuracy**
- 2: Reports close to **50%** in Sub-Saharan Africa and **at least 90%** in all other regions.
- 1: Gives approximate figures but incomplete comparison.
- 0: Reports household access or applies the Sub-Saharan Africa figure globally.

**Reasoning**
- 2: Distinguishes region grouping, school-level service definition, water-related services, and data-year/model status.
- 1: Mentions school/region but not enough to resolve comparability.
- 0: Confuses school water services with unrelated infrastructure indicators.

**Use of Evidence**
- 2: Uses official education indicator evidence and corroborates service-definition/date compatibility.
- 1: Uses one relevant source with limited comparison.
- 0: Uses general water-access statistics.

**Clarity and Structure**
- 2: Clear contrast between Sub-Saharan Africa and other regions with caveat/confidence.
- 1: Mostly clear but missing one section.
- 0: Unclear or broad water-access essay.

### Common Failure Modes

- Reporting household water access instead of school availability.
- Applying the Sub-Saharan Africa figure globally.
- Omitting the at-least-90% comparison for other regions.
- Ignoring service-definition differences.

### Borderline Cases

- Accept "about half" for close to 50% if the other-region comparison is exact enough.
- Do not require country-level breakdowns.
- If sanitation/hygiene is mentioned, it must not replace water-related service availability.

---

## 11. CORE-POL-03

rubric_id: CORE-RUBRIC-B04-CORE-POL-03
task_type: Core
research_object: OECD international protection grants
answer_unit: 676,000 refugees granted international protection in 2023 and 160,000 resettled refugees

### Key Facts From Source Bundle

- OECD countries granted international protection to **676,000 refugees in 2023**.
- The figure includes **160,000 new resettled refugees**.
- Protection grants are distinct from applications.
- Resettlement is distinct from other protection channels.
- OECD country coverage, reporting year, and revised totals matter.

### Expected Response Sections

- Conclusion with both figures and 2023 OECD coverage.
- Source comparison anchored in official migration/OECD evidence.
- Boundary explanation about grants/applications, resettlement channels, coverage, and reporting year.
- Caveat about revisions or definitions.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes both figures, coverage/year, category boundary, evidence, caveat, and confidence.
- 1: Gives both figures but omits resettlement/category boundary or caveat.
- 0: Omits one of the required figures.

**Accuracy**
- 2: Reports **676,000** protection grants in 2023 and **160,000** new resettled refugees.
- 1: Gives one correct figure and one incomplete/ambiguous figure.
- 0: Reports applications, total refugee stock, or wrong coverage.

**Reasoning**
- 2: Distinguishes protection grants, applications, resettlement, other channels, OECD coverage, and reporting year.
- 1: Mentions category distinctions but leaves one central boundary unclear.
- 0: Confuses refugees, migrants, applications, and resettlement.

**Use of Evidence**
- 2: Uses official migration/OECD evidence and corroborates definitions or revision status.
- 1: Uses one relevant source with limited comparison.
- 0: Uses incompatible asylum statistics without alignment.

**Clarity and Structure**
- 2: Clear two-figure answer with comparison, caveat, and confidence.
- 1: Mostly clear but incomplete.
- 0: Broad migration-policy answer.

### Common Failure Modes

- Reporting asylum applications instead of protection grants.
- Treating 160,000 as the total protected population.
- Omitting OECD coverage.
- Confusing refugees, migrants, and resettled refugees.

### Borderline Cases

- If "international protection" wording differs by source, score based on whether grants are clearly distinguished from applications.
- Later revisions should be caveated.
- Do not require non-OECD comparisons.

---

## 12. CORE-SCI-06

rubric_id: CORE-RUBRIC-B04-CORE-SCI-06
task_type: Core
research_object: young adults without upper-secondary attainment
answer_unit: 12% in the UK versus improvement from 17% to 14% across the comparison group

### Key Facts From Source Bundle

- The UK share of young adults without upper-secondary attainment was **12%**.
- The UK value stagnated between **2016 and 2023**.
- The comparison-group average improved from **17% to 14%**.
- The measure concerns young adults and upper-secondary attainment, not tertiary attainment.
- Age cohort, country classification, and comparability matter.

### Expected Response Sections

- Conclusion with the UK value/stagnation and comparison-group improvement.
- Source comparison anchored in official education/equity evidence.
- Boundary explanation about age cohort, attainment definition, country versus comparison average, and years.
- Caveat about classification/comparability.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes UK value, stagnation, comparison trend, years, evidence, caveat, and confidence.
- 1: Gives UK value but omits comparison trend or boundary detail.
- 0: Does not answer the attainment comparison.

**Accuracy**
- 2: Reports **12%** in the UK and comparison-group improvement from **17% to 14%**.
- 1: Gets one component correct or leaves stagnation/timing unclear.
- 0: Treats 12% as comparison average or reports tertiary attainment.

**Reasoning**
- 2: Distinguishes UK value, comparison-group average, age cohort, upper-secondary attainment, and reference years.
- 1: Mentions UK versus comparison but leaves cohort/definition unclear.
- 0: Conflates country value with group average or attainment levels.

**Use of Evidence**
- 2: Uses official education evidence and corroborates definition/year comparability.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated education-attainment figures.

**Clarity and Structure**
- 2: Clearly contrasts UK stagnation with comparison-group improvement.
- 1: Mostly clear but missing caveat or evidence comparison.
- 0: Unclear education-statistics discussion.

### Common Failure Modes

- Treating 12% as the comparison-group average.
- Reporting only the UK value and not the comparison trend.
- Confusing upper-secondary attainment with tertiary attainment.
- Ignoring age-cohort definition.

### Borderline Cases

- Partial credit if the answer gives the UK 12% but not stagnation.
- Do not require all comparison countries to be listed.
- If national classifications differ, reward answers that caveat comparability.

---

## 13. SET-TECH-E02

gold_set_id: SET-GOLD-B04-SET-TECH-E02
task_type: Set
research_object: Fire OS operating-system inventory entry
candidate_item: Fire OS
answer_unit: vendor or company grouping under which the candidate appears

### Correct Items

- Candidate item: **Fire OS**.
- Correct grouping: **Amazon** or the source's equivalent Amazon company/vendor heading.
- Required distinction: operating-system product versus vendor/company grouping.
- Required metadata: row entry and immediately preceding heading/grouping context.

### Acceptable Variants

- "Amazon", "Amazon.com", or source-equivalent Amazon vendor label.
- Notes that Fire OS is Android-derived if this is boundary context, not the requested grouping.
- Current/historical status notes if source-consistent.

### Optional Distractors

- Android as vendor grouping.
- Google.
- Device family or Fire tablet device label.
- Full operating-system list.

### Explicit Exclusion Rules

- Exclude "Android" when the requested field is vendor/company grouping.
- Exclude device-only answers.
- Exclude answers that ignore the row-versus-heading boundary.
- Exclude whole-list retrieval.

### Boundary Notes

- Precision/recall/F1 should use the bounded fields: candidate item, vendor/company grouping, row/heading source boundary.
- Android-derived family may be mentioned only as explanatory context.

---

## 14. SET-TECH-F05

gold_set_id: SET-GOLD-B04-SET-TECH-F05
task_type: Set
research_object: React web-framework comparison row
candidate_item: React
answer_unit: implementation language recorded for the candidate

### Correct Items

- Candidate item: **React**.
- Correct implementation language: **JavaScript** or the source's exact implementation-language wording.
- Required distinction: implementation language versus application authoring language.
- Required metadata: row field, version/date ambiguity if relevant.

### Acceptable Variants

- "JavaScript" if tied to the implementation-language field.
- Notes that developers may use JSX or TypeScript if these are not substituted for the recorded implementation language.
- Library/framework caveat if it does not replace the requested field.

### Optional Distractors

- TypeScript.
- JSX.
- HTML/CSS.
- Debates about library versus framework.
- Full framework list.

### Explicit Exclusion Rules

- Exclude TypeScript or JSX as the answer unless the controlling row explicitly records them.
- Exclude answers about languages used to write React applications instead of implementation language.
- Exclude responses that debate classification without giving the field value.
- Exclude whole-list retrieval.

### Boundary Notes

- Precision/recall/F1 should use candidate item, implementation-language field, and source row/version boundary.
- Classification as library/framework is a boundary note, not the answer unit.

---

## 15. BND-SET-SET007

gold_set_id: SET-GOLD-B04-BND-SET-SET007
task_type: Set
research_object: Tokyo largest-city population row
candidate_item: Tokyo
answer_unit: UN 2025 population estimate recorded for the candidate

### Correct Items

- Candidate row: **Tokyo**.
- Required value: the **UN 2025 population estimate** recorded for Tokyo in the controlling largest-city row.
- Required boundary: city proper, urban area, urban agglomeration, or metropolitan area as defined by the source row.
- Required metadata: estimate year 2025 and projection/source convention.

### Acceptable Variants

- Rounded population values if they match the controlling source's displayed units.
- "Tokyo urban agglomeration" or equivalent if that is the source boundary.
- Notes comparing city proper, prefecture, metro area, and urban agglomeration if the controlling row remains primary.

### Optional Distractors

- Tokyo prefecture population.
- Tokyo city-proper population.
- Greater Tokyo metropolitan area from another source.
- Current live city estimate.
- Full largest-city ranking.

### Explicit Exclusion Rules

- Exclude values for a different Tokyo boundary unless explicitly reconciled with the controlling row.
- Exclude answers omitting 2025/source convention when available.
- Exclude rankings instead of the candidate row value.
- Exclude whole-list retrieval.

### Boundary Notes

- Stable scoring requires a fixed controlling table version or source-consistent lookup-time value.
- Precision/recall/F1 should use candidate row, population value, 2025 estimate year, and geographic boundary.

---

## 16. BND-SET-SET012

gold_set_id: SET-GOLD-B04-BND-SET-SET012
task_type: Set
research_object: India English-speaking population row
candidate_item: India
answer_unit: total English-speaking population recorded for the candidate

### Correct Items

- Candidate row: **India**.
- Required value: total English-speaking population recorded for India in the controlling country row.
- Required boundary: total English speakers, not only native speakers.
- Required metadata: treatment of native/additional-language speakers, age group, survey year, and estimate/census status where available.

### Acceptable Variants

- Rounded totals if they match the source's displayed units.
- "English speakers in India" if it clearly means total speakers.
- Notes separating native, second-language, and additional-language speakers if the total remains primary.

### Optional Distractors

- Native English speakers only.
- Percentage without total population count.
- Current live estimate.
- Census-only figure from another year.
- Full country list.

### Explicit Exclusion Rules

- Exclude native-speaker-only answers as the total.
- Exclude percentage-only answers when the task asks for total population.
- Exclude mixed census/estimate years without explanation.
- Exclude whole-list retrieval.

### Boundary Notes

- Precision/recall/F1 should use candidate row, total-speaker value, speaker-type boundary, year, and source convention.
- Source updates should be handled by fixing the table version or accepting source-consistent lookup-time totals.
