# Batch 6 Evaluation Artifacts

Evaluation artifacts for the 16 runnable tasks in `manual_deep_research_batch_006.md`.

Phase 10 rule:
- Core tasks use a task-level rubric with five fixed criteria: Coverage, Accuracy, Reasoning, Use of evidence, Clarity and structure.
- Each Core criterion is scored 0-2, for 10 total points.
- Batch 6 contains Core tasks only; no Set gold sets are required.

---

## 1. BND-CORE-PAIR-054

rubric_id: CORE-RUBRIC-B06-BND-CORE-PAIR-054
task_type: Core
research_object: Netherlands regional working-age employment rates in 2023
answer_unit: national rate, regional range, and lowest/highest regions

### Key Facts From Source Bundle

- The employment rate is employed persons as a share of the working-age population aged **15-64**.
- The Netherlands national rate in 2023 is **82.3%**.
- The regional low is **79.1% in Limburg**.
- The regional high is **84.1% in North Brabant**.
- Regional values are distinct from the national rate.
- Differences should be treated as percentage-point values where compared, not relative percent changes.

### Expected Response Sections

- Conclusion with the national rate, low/high regional values, and region names.
- Source comparison anchored in the official regional employment source.
- Boundary explanation about employment rate, age scope, national versus regional values, and percentage points.
- Caveat about regional/source definitions and possible updates.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes national rate, regional low/high, regions, age boundary, evidence, caveat, and confidence.
- 1: Gives most values but omits age boundary, one region, or source comparison.
- 0: Does not answer the regional employment-rate question.

**Accuracy**
- 2: Reports **82.3% nationally**, **79.1% in Limburg**, and **84.1% in North Brabant**.
- 1: Gets two values correct or gives all values with unclear region mapping.
- 0: Reports unemployment, participation, or swaps the low/high regions.

**Reasoning**
- 2: Distinguishes employment/unemployment/participation, ages 15-64/total population, national/regional values, and percentage points/percent change.
- 1: Mentions one or two boundaries but leaves comparability unclear.
- 0: Conflates measures or population scopes.

**Use of Evidence**
- 2: Uses the official regional employment source and compares only compatible labour data.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported labour statistics or incompatible regional definitions.

**Clarity and Structure**
- 2: Clear rate/range answer with comparison, caveat, and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing labour-market summary.

### Common Failure Modes

- Reporting unemployment instead of employment.
- Using total population rather than ages 15-64.
- Swapping Limburg and North Brabant.
- Omitting the national rate or regional range.

### Borderline Cases

- Partial credit is appropriate if the values are rounded but region mapping is correct.
- Do not require a full regional table.
- If a later source updates regional values, it must be caveated against the 2023 source context.

---

## 2. BND-CORE-PAIR-019

rubric_id: CORE-RUBRIC-B06-BND-CORE-PAIR-019
task_type: Core
research_object: Korea labour-market status in May 2024
answer_unit: employment rate and comparison with May 2023 and December 2019

### Key Facts From Source Bundle

- Korea's employment rate for people aged **15-64** was **69.4% in May 2024**.
- This was the same as in **May 2023**.
- It was **2.2 percentage points above December 2019**.
- The measure is employment rate, not unemployment or participation.
- The 15-64 age boundary must be preserved.
- Seasonal adjustment or source-definition differences may matter.

### Expected Response Sections

- Conclusion with May 2024 rate and comparisons to May 2023 and December 2019.
- Source comparison anchored in the official labour-market note.
- Boundary explanation about employment/unemployment, age coverage, unchanged level, and percentage-point increase.
- Caveat about adjustment and source definitions.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes rate, age group, both comparisons, evidence, caveat, and confidence.
- 1: Gives the rate but omits one comparison or boundary.
- 0: Does not answer Korea's employment-rate status.

**Accuracy**
- 2: Reports **69.4% in May 2024**, same as May 2023, and **2.2 percentage points above December 2019**.
- 1: Gets the rate and one comparison correct.
- 0: Reports unemployment or uses all-adult coverage without support.

**Reasoning**
- 2: Distinguishes employment/unemployment/participation, 15-64/all adults, unchanged level, and percentage-point change.
- 1: Mentions one boundary but leaves another important distinction unclear.
- 0: Treats 2.2 percentage points as a relative percent increase or different measure.

**Use of Evidence**
- 2: Uses the official labour-market source and corroborates only compatible definitions/update status.
- 1: Uses one relevant source with limited comparison.
- 0: Uses incompatible labour data without explanation.

**Clarity and Structure**
- 2: Clearly states rate and both comparisons with caveat/confidence.
- 1: Mostly clear but incomplete.
- 0: Unclear or broad labour-market discussion.

### Common Failure Modes

- Reporting unemployment or labour-force participation.
- Treating 2.2 percentage points as a relative percent increase.
- Omitting the May 2023 comparison.
- Using all-adult rather than 15-64 coverage.

### Borderline Cases

- Accept "unchanged from a year earlier" as the May 2023 comparison.
- If seasonally adjusted status is unknown, the answer should caveat rather than invent it.
- Country naming variants for Korea are acceptable if the source context is clear.

---

## 3. CORE-POL-04

rubric_id: CORE-RUBRIC-B06-CORE-POL-04
task_type: Core
research_object: occupation-shortage evidence for health and social care
answer_unit: period and evidence basis used to identify shortages

### Key Facts From Source Bundle

- Shortage evidence covers the period **2022 and 2023**.
- The sector focus is health and social care.
- The evidence draws on diverse sources and indicators.
- Public employment services' administrative data are included among the evidence sources.
- Shortage evidence is distinct from employment totals.
- The evidence period is distinct from later policy responses.

### Expected Response Sections

- Conclusion with the 2022-2023 period and evidence basis.
- Source comparison anchored in the official workforce/policy source.
- Boundary explanation about shortage evidence, sector scope, administrative data, and policy responses.
- Caveat about indicator diversity and source comparability.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes period, sector, diverse evidence basis, administrative data, evidence, caveat, and confidence.
- 1: Includes period but omits sector or evidence-basis detail.
- 0: Does not answer period/evidence basis.

**Accuracy**
- 2: States **2022 and 2023** and diverse sources including **public employment services' administrative data**.
- 1: Gives the period but weakly describes evidence sources.
- 0: Gives current shortages only or employment totals.

**Reasoning**
- 2: Distinguishes shortage evidence, employment totals, health/social care sector, administrative indicators, survey perceptions, and later policies.
- 1: Mentions one boundary but leaves evidence type unclear.
- 0: Generalises to all occupations or treats administrative data as the only basis.

**Use of Evidence**
- 2: Uses the official workforce source and corroborates only compatible shortage-indicator context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsourced labour-market claims.

**Clarity and Structure**
- 2: Concise period-plus-evidence answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Broad shortage essay without answer unit.

### Common Failure Modes

- Giving current shortages without the 2022-2023 evidence period.
- Treating administrative data as the only evidence source.
- Reporting employment headcounts instead of shortage evidence.
- Generalising to all occupations or sectors.

### Borderline Cases

- Accept "spanning 2022-2023" as equivalent.
- Partial credit if administrative data are named but other indicators are not.
- Do not require listing every evidence source if diversity and administrative data are clear.

---

## 4. CORE-SCI-02

rubric_id: CORE-RUBRIC-B06-CORE-SCI-02
task_type: Core
research_object: education-attainment gender gap among young adults
answer_unit: young women and young men tertiary-qualification shares

### Key Facts From Source Bundle

- **54% of young women** hold a tertiary qualification.
- **41% of young men** hold a tertiary qualification.
- The population is young adults, not all adults.
- Tertiary qualification is distinct from tertiary enrolment and upper-secondary completion.
- The gap should be framed as a percentage-point difference if calculated.
- Source scope may be cross-country aggregate or source-specific and should be stated.

### Expected Response Sections

- Conclusion with both gender shares.
- Source comparison anchored in the official education indicator source.
- Boundary explanation about young adults, tertiary attainment, and percentage-point gap.
- Caveat about aggregate/source scope and comparability.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes both shares, population/measure boundary, evidence, caveat, and confidence.
- 1: Gives both shares but omits boundary or source scope.
- 0: Does not answer the gender-share question.

**Accuracy**
- 2: Reports **54% young women** and **41% young men**.
- 1: Gets one value correct or gives the gap without both shares.
- 0: Swaps values or reports enrolment/all-adult attainment.

**Reasoning**
- 2: Distinguishes young/all adults, tertiary/upper-secondary, attainment/enrolment, and percentage-point/relative gap.
- 1: Mentions one distinction but leaves scope unclear.
- 0: Conflates attainment levels or age groups.

**Use of Evidence**
- 2: Uses official education indicators and corroborates compatible demographic/attainment definitions.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated education statistics.

**Clarity and Structure**
- 2: Clear gender comparison with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Unclear education-attainment discussion.

### Common Failure Modes

- Swapping the male and female values.
- Reporting tertiary enrolment instead of attainment.
- Applying the figures to all adults.
- Omitting the gender comparison.

### Borderline Cases

- If the answer calculates a 13 percentage-point gap, it must still include the two shares for full coverage.
- Do not require country-level breakdowns unless the source scope is country-specific.
- "Women" and "men" are acceptable shorthand if young-adult scope is stated.

---

## 5. CORE-SCI-16

rubric_id: CORE-RUBRIC-B06-CORE-SCI-16
task_type: Core
research_object: child overweight and obesity regional distribution in 2024
answer_unit: Africa increase since 2000 and Asia share of under-5 cases

### Key Facts From Source Bundle

- The number of overweight children under 5 in Africa increased by **nearly 12.1% since 2000**.
- Almost half of children under 5 who were overweight or living with obesity in 2024 lived in **Asia**.
- The age boundary is children under 5.
- Overweight and obesity-only measures should not be conflated.
- Regional counts are distinct from prevalence rates.
- The Africa change since 2000 is distinct from the 2024 regional distribution.

### Expected Response Sections

- Conclusion with Africa's nearly 12.1% increase and Asia's almost-half share.
- Source comparison anchored in the official child-health indicator source.
- Boundary explanation about age group, overweight/obesity, regional counts/prevalence, and time period.
- Caveat about estimates and regional comparability.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes both regional facts, age/measure boundaries, evidence, caveat, and confidence.
- 1: Includes one regional fact fully and the other partially.
- 0: Does not answer the regional distribution/change question.

**Accuracy**
- 2: Reports Africa increased by **nearly 12.1% since 2000** and Asia had **almost half** of under-5 overweight/obesity cases in 2024.
- 1: Gets one component correct or leaves the other imprecise.
- 0: Reports adolescent obesity or treats 12.1% as prevalence.

**Reasoning**
- 2: Distinguishes overweight/obesity-only, under-5/older children, regional counts/prevalence, and 2024 distribution/long-run change.
- 1: Mentions one boundary but leaves comparability unclear.
- 0: Conflates prevalence, counts, age groups, or regions.

**Use of Evidence**
- 2: Uses official health indicator evidence and corroborates only compatible estimates/definitions.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated obesity statistics.

**Clarity and Structure**
- 2: Clear two-part regional answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Broad child-health discussion.

### Common Failure Modes

- Reporting adolescent obesity instead of under-5 figures.
- Treating 12.1% as a prevalence rate.
- Saying Asia has half of all children, not under-5 overweight/obesity cases.
- Omitting either Africa or Asia.

### Borderline Cases

- Accept "about half" for "almost half."
- Partial credit if the answer says "overweight children" but does not mention living with obesity, if the boundary is otherwise clear.
- Do not require exact Asia percentage if the source only gives a qualitative share.

---

## 6. BND-CORE-PAIR-046

rubric_id: CORE-RUBRIC-B06-BND-CORE-PAIR-046
task_type: Core
research_object: macroeconomic imbalance scoreboard export-performance indicator
answer_unit: 2024 status change and threshold

### Key Facts From Source Bundle

- Export performance against advanced economies was upgraded from **auxiliary** to **headline** indicator.
- This occurred in the **2024** scoreboard review.
- The indicator is measured as a **three-year change**.
- The newly established threshold is **-3%**.
- Export performance against advanced economies is distinct from export market share generally.
- A threshold breach is not an automatic policy conclusion.

### Expected Response Sections

- Conclusion with status change, measurement period, and threshold.
- Source comparison anchored in the official scoreboard review.
- Boundary explanation about headline/auxiliary status, comparator, three-year change, and threshold meaning.
- Caveat about methodology-review context.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes status change, year, three-year measure, threshold, evidence, caveat, and confidence.
- 1: Gives threshold/status but omits measurement period or caveat.
- 0: Does not answer status change and threshold.

**Accuracy**
- 2: Reports auxiliary-to-headline upgrade, **three-year change**, and **-3%** threshold.
- 1: Gets threshold and status but not measurement period.
- 0: Treats -3% as a country result or reports another indicator.

**Reasoning**
- 2: Distinguishes headline/auxiliary status, advanced-economy comparator, three-year/annual measure, and threshold/policy conclusion.
- 1: Mentions one boundary but leaves indicator meaning unclear.
- 0: Conflates the threshold with observed export growth.

**Use of Evidence**
- 2: Uses official scoreboard-review evidence and corroborates only compatible methodology updates.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported MIP summaries or wrong indicator material.

**Clarity and Structure**
- 2: Clear methodology/status conclusion with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing scoreboard discussion.

### Common Failure Modes

- Treating -3% as a country result.
- Ignoring the auxiliary-to-headline status change.
- Reporting annual export growth instead of three-year change.
- Confusing the threshold with another scoreboard indicator.

### Borderline Cases

- Accept "minus three percent" as equivalent.
- This overlaps with earlier MIP threshold tasks; score consistently while requiring the status-change component here.
- Do not require country examples.

---

## 7. BND-CORE-PAIR-042

rubric_id: CORE-RUBRIC-B06-BND-CORE-PAIR-042
task_type: Core
research_object: digital-service progression maturity metric
answer_unit: baseline, latest result, and maturity level

### Key Facts From Source Bundle

- The progression maturity metric baseline is **24% in 2020**.
- The latest known result is **40%**.
- The maturity label is **Level 2 - Reactive**.
- There is a target to increase by the end of 2024.
- Baseline, target, and latest result are distinct.
- The percentage metric is distinct from the maturity-level label.
- This internal metric is distinct from broader digital-government maturity.

### Expected Response Sections

- Conclusion with baseline, latest result, maturity level, and target caveat.
- Source comparison anchored in official/internal annual reporting.
- Boundary explanation about baseline/latest/target and percentage/level label.
- Caveat about achieved status versus end-2024 target.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes baseline, latest result, maturity label, target status, evidence, caveat, and confidence.
- 1: Includes most metrics but omits target or maturity label.
- 0: Does not answer the progression metric question.

**Accuracy**
- 2: Reports **24% baseline in 2020**, **40% latest result**, and **Level 2 - Reactive**.
- 1: Gets two components correct.
- 0: Reports 40% as target or omits the maturity level entirely.

**Reasoning**
- 2: Distinguishes percentage metric/maturity label, baseline/target/latest result, achieved/target status, and internal/broader maturity.
- 1: Mentions one distinction but leaves target/result unclear.
- 0: Conflates target with achieved status or unrelated maturity models.

**Use of Evidence**
- 2: Uses official reporting evidence and corroborates only compatible metric/status context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic digital-government maturity material.

**Clarity and Structure**
- 2: Clear metric table-style answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing digital-service answer.

### Common Failure Modes

- Reporting 40% as the target rather than latest result.
- Omitting the Level 2 - Reactive label.
- Treating target increase as achieved.
- Confusing this metric with open-data maturity or service availability.

### Borderline Cases

- "Reactive level 2" is acceptable wording.
- Do not require exact target value if the prompt only asks baseline/latest/maturity and target status.
- Later results must be identified as updates, not substituted silently.

---

## 8. BND-CORE-PAIR-035

rubric_id: CORE-RUBRIC-B06-BND-CORE-PAIR-035
task_type: Core
research_object: cohesion-policy performance-data reliability in 2024
answer_unit: whether reliability deficiencies led to suspension of interim payments

### Key Facts From Source Bundle

- Performance-data reliability deficiencies are closely followed up.
- Such deficiencies can lead to suspension of interim payments.
- **No such procedure was launched in 2024**.
- Potential suspension authority is distinct from an actual launched procedure.
- Performance-data reliability is distinct from financial error rate.
- Interim payments are distinct from programme selection or approval.

### Expected Response Sections

- Conclusion stating the potential consequence and 2024 non-launch status.
- Source comparison anchored in official annual/control reporting.
- Boundary explanation about potential authority versus actual procedure, performance data versus financial errors, and interim payments.
- Caveat about 2024-specific status and later audit outcomes.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes potential suspension, no 2024 procedure, payment type, evidence, caveat, and confidence.
- 1: Gives status but omits potential/actual distinction or payment boundary.
- 0: Does not answer whether suspension occurred.

**Accuracy**
- 2: States deficiencies can lead to suspension but **no such procedure was launched in 2024**.
- 1: Says no suspension in 2024 but weakly handles the authority.
- 0: Says payments were suspended in 2024.

**Reasoning**
- 2: Distinguishes potential/actual procedure, performance-data reliability/financial error rate, 2024/later status, and interim payments/programme approval.
- 1: Mentions one distinction but leaves procedural status unclear.
- 0: Conflates reliability deficiencies with audit error rates or payment suspension.

**Use of Evidence**
- 2: Uses official control/reporting evidence and corroborates only compatible status/legal context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported audit claims or later years without caveat.

**Clarity and Structure**
- 2: Clear legal/status conclusion with comparison, caveat, and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing cohesion-policy control answer.

### Common Failure Modes

- Saying payments were suspended in 2024.
- Ignoring the "can lead to" versus "did lead to" distinction.
- Confusing performance-data reliability with audit error rates.
- Extending the 2024 finding to later years without evidence.

### Borderline Cases

- "No procedure launched" and "no suspension procedure initiated" are equivalent.
- Do not require detailed legal procedure description.
- Later audit developments should be caveated separately.

---

## 9. BND-CORE-PAIR-001

rubric_id: CORE-RUBRIC-B06-BND-CORE-PAIR-001
task_type: Core
research_object: industrial-equipment company 2024 proposed dividend
answer_unit: proposed dividend per share and increase versus previous year

### Key Facts From Source Bundle

- The proposed dividend for financial year 2024 is **EUR 1.15 per share**.
- This is an increase of **15 cents** over the previous year.
- The dividend is proposed, not necessarily approved or paid at the source point.
- Per-share amount is distinct from total payout.
- Euro-cent increase is distinct from percentage increase.
- Later shareholder approval should be caveated.

### Expected Response Sections

- Conclusion with proposed per-share dividend and cent increase.
- Source comparison anchored in the official company report.
- Boundary explanation about proposed/paid/approved, per-share/total payout, and cents/percent.
- Caveat about later approval.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes amount, increase, proposal status, evidence, caveat, and confidence.
- 1: Gives amount and increase but omits proposal/status caveat.
- 0: Does not answer the proposed dividend question.

**Accuracy**
- 2: Reports **EUR 1.15 per share** and **15-cent** increase.
- 1: Gets one component correct or gives amount with unclear per-share status.
- 0: Treats EUR 1.15 as total payout or reports previous year's dividend.

**Reasoning**
- 2: Distinguishes proposed/paid/approved, per-share/total payout, cents/percentage increase, and financial-year/later approval.
- 1: Mentions one distinction but leaves status unclear.
- 0: Conflates proposal with paid dividend or total payout.

**Use of Evidence**
- 2: Uses official company reporting and corroborates only compatible approval/update status.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported finance snippets or unrelated dividend data.

**Clarity and Structure**
- 2: Clear dividend answer with comparison, caveat, and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing shareholder-return discussion.

### Common Failure Modes

- Treating EUR 1.15 as total payout.
- Reporting the previous year's dividend instead.
- Converting 15 cents into an unsupported percentage.
- Omitting proposed status.

### Borderline Cases

- Accept "€1.15" as equivalent.
- Later shareholder approval may be mentioned only as update context.
- If the answer calculates a percentage increase, it must not replace the 15-cent answer unit.

---

## 10. CORE-POL-36

rubric_id: CORE-RUBRIC-B06-CORE-POL-36
task_type: Core
research_object: Spain open-data reuse-frequency survey
answer_unit: 2023 low-use share and missing-response caveat

### Key Facts From Source Bundle

- In 2023, **29%** reported using open data **sometimes or almost never**.
- **58%** of respondents did not answer the question.
- "Sometimes or almost never" is distinct from frequent use.
- Respondent share is distinct from population share.
- Non-response is distinct from zero use.
- The value is a 2023 survey result, not a 2021 or 2019 comparison.

### Expected Response Sections

- Conclusion with the 29% low-use share and 58% non-response caveat.
- Source comparison anchored in the official country response.
- Boundary explanation about use frequency, respondent base, non-response, and survey year.
- Caveat about survey limitations and missing responses.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes both percentages, survey year, response boundary, evidence, caveat, and confidence.
- 1: Gives both percentages but omits non-response interpretation or source comparison.
- 0: Does not answer the reuse-frequency survey question.

**Accuracy**
- 2: Reports **29% sometimes/almost never** and **58% did not answer**.
- 1: Gets one percentage correct or weakly labels response status.
- 0: Treats 58% as non-users or reports open-data awareness.

**Reasoning**
- 2: Distinguishes low/frequent use, respondent/population share, non-response/zero use, and 2023/earlier comparisons.
- 1: Mentions one boundary but leaves survey interpretation unclear.
- 0: Treats survey respondents as the whole population or non-response as non-use.

**Use of Evidence**
- 2: Uses the official country response and corroborates only compatible survey/context information.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated open-data survey claims.

**Clarity and Structure**
- 2: Clear survey answer with non-response caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Unclear open-data usage narrative.

### Common Failure Modes

- Treating 58% as non-users.
- Omitting the non-response caveat.
- Reporting open-data awareness instead of reuse frequency.
- Treating survey respondents as the whole population.

### Borderline Cases

- Accept "rarely or sometimes" if it clearly maps to the source category.
- Do not require earlier-year comparisons.
- If 58% is described as missing response, that is valid even without deeper survey methodology.

---

## 11. BND-CORE-PAIR-032

rubric_id: CORE-RUBRIC-B06-BND-CORE-PAIR-032
task_type: Core
research_object: open-data impact survey methodology
answer_unit: 2023 survey basis and impact dimensions covered

### Key Facts From Source Bundle

- A **2023 open-data impact survey** was conducted.
- It used a national methodology inspired by European work.
- It covers **outputs, outcomes, and impacts**.
- Coverage spans **four dimensions**.
- Survey methodology is distinct from measured impact results.
- The national method is distinct from a cross-country framework.
- The 2023 survey is distinct from earlier impact studies.

### Expected Response Sections

- Conclusion with 2023 survey basis and covered impact dimensions.
- Source comparison anchored in the official country response.
- Boundary explanation about methodology/results, outputs/outcomes/impacts, national/cross-country methods, and survey timing.
- Caveat about what the survey does and does not prove.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes survey year, methodology basis, outputs/outcomes/impacts, four dimensions, evidence, caveat, and confidence.
- 1: Gives survey year and dimensions but omits methodology basis or caveat.
- 0: Does not answer survey methodology.

**Accuracy**
- 2: States a **2023** survey, national methodology inspired by European work, covering outputs, outcomes, and impacts across four dimensions.
- 1: Gets most components but omits one key element.
- 0: Reports impact findings instead of methodology scope.

**Reasoning**
- 2: Distinguishes methodology/results, outputs/outcomes/impacts, national/cross-country method, and 2023/earlier studies.
- 1: Mentions one distinction but leaves scope unclear.
- 0: Confuses outputs, outcomes, and impacts or treats method as measured result.

**Use of Evidence**
- 2: Uses the official country response and corroborates only methodology/source-context details.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic open-data impact frameworks without the country survey.

**Clarity and Structure**
- 2: Clear methodology answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Broad open-data impact essay.

### Common Failure Modes

- Reporting impact findings instead of methodology scope.
- Omitting the four-dimension coverage.
- Treating the national method as identical to a cross-country framework.
- Confusing outputs, outcomes, and impacts.

### Borderline Cases

- If the four dimensions are not named, full credit is still possible if the answer correctly states that four dimensions are covered and the prompt did not require names.
- Do not require numeric impact results.
- Later surveys should be caveated separately.

---

## 12. CORE-POL-26

rubric_id: CORE-RUBRIC-B06-CORE-POL-26
task_type: Core
research_object: open-data-supported pharmaceutical investigation
answer_unit: estimated value and role of official drug-control data

### Key Facts From Source Bundle

- The investigation uncovered illegal pharmaceutical activity worth **EUR 20 million**.
- The investigation used analysis of open data from the official/state drug-control body.
- Many drugs ended up in pharmacies abroad.
- Estimated value is distinct from recovered value.
- Official drug-control open data are distinct from investigative conclusions.
- A reuse-case description is not necessarily a final legal/court outcome.

### Expected Response Sections

- Conclusion with estimated value and role of official drug-control data.
- Source comparison anchored in the official country response.
- Boundary explanation about estimated/recovered value, data source/investigative finding, and domestic/foreign pharmacy flows.
- Caveat about legal outcome status.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes EUR 20 million, data source role, foreign-pharmacy detail, evidence, caveat, and confidence.
- 1: Gives value and data source but omits caveat or destination detail.
- 0: Does not answer the investigation value/data role.

**Accuracy**
- 2: Reports **EUR 20 million** illegal pharmaceutical activity, based on official drug-control open data, with drugs ending up in pharmacies abroad.
- 1: Gets value and broad data role but imprecise detail.
- 0: Reports EUR 20 million as recovered funds or court award.

**Reasoning**
- 2: Distinguishes estimated/recovered value, data source/conclusion, domestic flow/foreign destination, and reuse case/legal outcome.
- 1: Mentions one boundary but leaves legal/value status unclear.
- 0: Treats reuse case as final court verdict or recovered amount.

**Use of Evidence**
- 2: Uses the official country response and corroborates only compatible investigation/context details.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported crime or pharmaceutical-market claims.

**Clarity and Structure**
- 2: Clear concise investigation answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Unfocused pharmaceutical-crime narrative.

### Common Failure Modes

- Reporting EUR 20 million as recovered funds.
- Omitting the role of official drug-control data.
- Treating the reuse case as a court verdict.
- Ignoring the foreign-pharmacy destination detail.

### Borderline Cases

- Accept "state drug agency/body" if it clearly refers to the official drug-control source.
- The foreign-pharmacy detail can be partial if the value and data role are precise.
- Do not require naming individual pharmacies or defendants.

---

## 13. CORE-POL-35

rubric_id: CORE-RUBRIC-B06-CORE-POL-35
task_type: Core
research_object: open-data portal API analytics tooling
answer_unit: tool change from 2024 and API-usage monitoring status

### Key Facts From Source Bundle

- API usage analytics are monitored.
- **Google Analytics** was used until 2024.
- **Matomo** was used after the 2024 change.
- API analytics are distinct from general website analytics.
- Tool migration is distinct from simultaneous tool use unless the source says otherwise.
- "Until 2024" should be handled carefully, not assumed to mean full-year coverage.
- Monitoring status is distinct from public reporting of metrics.

### Expected Response Sections

- Conclusion with monitoring status and tool change.
- Source comparison anchored in the official country response.
- Boundary explanation about API/general analytics, tool migration, timing, and public reporting.
- Caveat about "until 2024" timing.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes monitoring status, both tools, timing, evidence, caveat, and confidence.
- 1: Includes tools but omits monitoring/timing caveat.
- 0: Does not answer API analytics tooling.

**Accuracy**
- 2: States API usage analytics are monitored; **Google Analytics until 2024**, then **Matomo**.
- 1: Names both tools but unclear sequence or monitoring status.
- 0: Says API usage is not monitored or omits one tool.

**Reasoning**
- 2: Distinguishes API/general analytics, migration/parallel use, until-2024/full-year coverage, and monitoring/public reporting.
- 1: Mentions one boundary but leaves timing unclear.
- 0: Treats tool change as a metric result.

**Use of Evidence**
- 2: Uses official country response and corroborates only compatible portal/tool status.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic analytics-tool information.

**Clarity and Structure**
- 2: Clear monitoring/tool timeline with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing portal analytics answer.

### Common Failure Modes

- Saying API usage is not monitored.
- Omitting one of the two tools.
- Treating the tool change as a metric result.
- Confusing API analytics with dataset downloads generally.

### Borderline Cases

- "GA" is acceptable if expanded or unambiguous.
- If the exact cutover date is unknown, a caveat is better than overclaiming.
- Do not require actual API usage numbers.

---

## 14. CORE-TECH-06

rubric_id: CORE-RUBRIC-B06-CORE-TECH-06
task_type: Core
research_object: AI risk measurement and monitoring practice
answer_unit: tracking mechanism requirement under the risk-measurement function

### Key Facts From Source Bundle

- The risk-measurement function calls for mechanisms to track identified AI risks over time.
- Related practices include ongoing monitoring.
- Related practices include periodic updates.
- Related practices include testing.
- Related practices include expert recalibration.
- Related practices include tracking incidents or errors.
- Risk measurement is distinct from risk mapping or risk management.
- Framework outcomes are not automatically binding legal obligations.

### Expected Response Sections

- Conclusion describing the tracking mechanism requirement.
- Source comparison anchored in the controlling AI risk-management framework.
- Boundary explanation about measurement/mapping/management, over-time tracking, monitoring, and legal status.
- Caveat about framework status and implementation context.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes over-time tracking, monitoring/update/testing/recalibration/incident elements, evidence, caveat, and confidence.
- 1: Gives tracking requirement but omits several linked practices or framework caveat.
- 0: Does not answer the tracking requirement.

**Accuracy**
- 2: States mechanisms should track identified AI risks over time under risk measurement, linked to ongoing monitoring, updates, testing, expert recalibration, and incidents/errors.
- 1: States tracking over time but misses some linked elements.
- 0: Summarises the whole framework or claims a binding legal duty without support.

**Reasoning**
- 2: Distinguishes risk measurement/mapping/management, over-time/one-time testing, operational monitoring/pre-deployment validation, and framework/legal duty.
- 1: Mentions one distinction but leaves function scope unclear.
- 0: Treats monitoring as a one-time assessment or legal requirement by default.

**Use of Evidence**
- 2: Uses the controlling framework source and corroborates only compatible framework interpretation.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic AI governance advice.

**Clarity and Structure**
- 2: Clear framework-function answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Unfocused AI-risk framework summary.

### Common Failure Modes

- Summarising the whole AI framework instead of the tracking requirement.
- Treating monitoring as a one-time assessment.
- Omitting incidents/errors or periodic updates.
- Claiming binding legal duty without support.

### Borderline Cases

- Do not require exact framework labels if risk-measurement function is clear.
- Partial credit is appropriate if incidents/errors are omitted but tracking over time is correct.
- Legal comparisons are acceptable only if they preserve framework status.

---

## 15. CORE-TECH-12

rubric_id: CORE-RUBRIC-B06-CORE-TECH-12
task_type: Core
research_object: federated learning privacy-preserving training model
answer_unit: core mechanism for collaborative training without raw-data transfer

### Key Facts From Source Bundle

- Federated learning enables collaborative training of machine-learning models.
- Raw, potentially sensitive data stay local rather than being transferred to a central pool.
- Model updates, parameters, or gradients may still be exchanged.
- Privacy-preserving does not mean a formal or absolute privacy guarantee by itself.
- The answer should describe the general mechanism, not one deployment architecture.
- Federated learning is distinct from encrypted centralised training.

### Expected Response Sections

- Conclusion explaining collaborative training without raw-data transfer.
- Source comparison anchored in the primary federated-learning survey.
- Boundary explanation about local raw data, exchanged updates, centralised pooling, and privacy limits.
- Caveat about privacy guarantees and deployment variants.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes collaborative training, local raw data, exchanged updates, privacy caveat, evidence, and confidence.
- 1: Explains local data but omits update exchange or privacy caveat.
- 0: Does not describe federated learning's mechanism.

**Accuracy**
- 2: Correctly states collaborative model training occurs without transferring raw data to a central pool.
- 1: Gives a broadly correct definition but overstates privacy or omits collaboration.
- 0: Says no information leaves devices at all or describes centralised training.

**Reasoning**
- 2: Distinguishes federated/centralised training, privacy preservation/formal guarantees, updates/raw data, and general mechanism/specific architecture.
- 1: Mentions one boundary but leaves privacy or update exchange unclear.
- 0: Treats privacy preservation as absolute anonymity.

**Use of Evidence**
- 2: Uses the primary survey source and corroborates only compatible definitions or caveats.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated privacy technology descriptions.

**Clarity and Structure**
- 2: Clear mechanism explanation with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing or overbroad ML privacy answer.

### Common Failure Modes

- Saying no information leaves local devices at all.
- Confusing federated learning with encrypted centralised training.
- Treating privacy preservation as absolute anonymity.
- Omitting collaborative model training.

### Borderline Cases

- "Model updates" can include gradients/parameters if used accurately.
- Do not require a detailed algorithm.
- Additional privacy techniques may be mentioned only as optional enhancements.

---

## 16. CORE-TECH-15

rubric_id: CORE-RUBRIC-B06-CORE-TECH-15
task_type: Core
research_object: low-bit large-language-model quantization tradeoff
answer_unit: efficiency benefit and information-loss risk

### Key Facts From Source Bundle

- Low-bit quantization can bring significant inference acceleration.
- It can also provide parameter compression.
- It may cause information loss.
- Parameter compression is distinct from runtime speedup.
- Inference quantization is distinct from training-time quantization.
- Information loss is distinct from measured accuracy degradation unless the source gives both.
- The answer should not reduce the issue to one algorithm or hardware implementation.

### Expected Response Sections

- Conclusion with efficiency benefits and information-loss risk.
- Source comparison anchored in the primary low-bit LLM survey.
- Boundary explanation about compression/speedup, inference/training quantization, and information loss/accuracy.
- Caveat about method, model, and hardware dependence.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes acceleration, compression, information loss, methodological boundaries, evidence, caveat, and confidence.
- 1: Includes benefits but omits information-loss caveat or one boundary.
- 0: Does not answer the quantization tradeoff.

**Accuracy**
- 2: States low-bit quantization can accelerate inference and compress parameters but may cause information loss.
- 1: Gives benefits and a vague risk.
- 0: Claims quantization always improves quality or omits the risk.

**Reasoning**
- 2: Distinguishes compression/speedup, inference/training quantization, information loss/accuracy degradation, and general method/specific implementation.
- 1: Mentions one distinction but leaves tradeoff unclear.
- 0: Confuses quantization with pruning/distillation or treats information loss as guaranteed accuracy drop.

**Use of Evidence**
- 2: Uses the primary survey source and corroborates only compatible technical findings.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated optimization claims.

**Clarity and Structure**
- 2: Clear benefit-risk answer with source comparison, caveat, and confidence.
- 1: Mostly clear but incomplete.
- 0: Unfocused LLM efficiency answer.

### Common Failure Modes

- Claiming quantization always improves quality.
- Reporting only compression and omitting information loss.
- Treating information loss as a guaranteed measured accuracy drop.
- Confusing low-bit quantization with pruning or distillation.

### Borderline Cases

- "Reduced memory footprint" is acceptable as parameter compression if the relation is clear.
- Mentioning accuracy degradation is acceptable only if it is framed as a possible consequence or source-supported measurement.
- Do not require naming a specific quantization algorithm.
