# Batch 9 Evaluation Artifacts

Evaluation artifacts for the 16 runnable tasks in `manual_deep_research_batch_009.md`.

Phase 10 rule:
- Core tasks use a task-level rubric with five fixed criteria: Coverage, Accuracy, Reasoning, Use of evidence, Clarity and structure.
- Each Core criterion is scored 0-2, for 10 total points.
- Batch 9 contains Core tasks only; no Set gold sets are required.

---

## 1. BND-CORE-PAIR-005

rubric_id: CORE-RUBRIC-B09-BND-CORE-PAIR-005
task_type: Core
research_object: restricted-stock-unit vesting schedule
answer_unit: first-anniversary vesting share and later vesting share

### Key Facts From Source Bundle

- Time-based restricted stock units have **25%** eligible to vest on the first anniversary of employment.
- The remaining **75%** are eligible to vest over the rest of the four-year period.
- Time-based vesting is distinct from performance awards.
- First-anniversary eligibility is distinct from grant-date ownership.
- Percentages refer to units, not dollar value.
- Termination or special-award exceptions may alter the standard schedule.

### Expected Response Sections

- Conclusion with the 25% first-anniversary share and remaining 75% schedule.
- Source comparison anchored in the official company award document.
- Boundary explanation about time-based vesting, eligibility, unit percentages, and exceptions.
- Caveat about termination or special-award terms.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes both vesting shares, four-year schedule, award type, evidence, caveat, and confidence.
- 1: Gives both shares but omits schedule or caveat.
- 0: Does not answer the vesting schedule.

**Accuracy**
- 2: Reports **25%** eligible on first anniversary and remaining **75%** over the rest of the four-year period.
- 1: Gets one share correct or states the schedule ambiguously.
- 0: Says all units vest after one year or reports dollar compensation.

**Reasoning**
- 2: Distinguishes time-based/performance awards, eligibility/ownership, unit percentages/dollar values, and standard schedule/exceptions.
- 1: Mentions one boundary but leaves vesting meaning unclear.
- 0: Treats vesting eligibility as immediate ownership.

**Use of Evidence**
- 2: Uses the official award document and corroborates only compatible award-term details.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic equity-compensation summaries.

**Clarity and Structure**
- 2: Clear schedule answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing compensation answer.

### Common Failure Modes

- Saying all units vest after one year.
- Treating vesting eligibility as immediate ownership.
- Reporting dollar compensation instead of unit percentages.
- Ignoring the remaining 75% schedule.

### Borderline Cases

- "One quarter" and "three quarters" are acceptable.
- Do not require every termination exception.
- Special-award exceptions should be caveated, not treated as the standard schedule.

---

## 2. BND-CORE-PAIR-009

rubric_id: CORE-RUBRIC-B09-BND-CORE-PAIR-009
task_type: Core
research_object: global disinflation resilience narrative
answer_unit: direction of inflation and activity during 2022-2023

### Key Facts From Source Bundle

- Global inflation descended from its **mid-2022 peak** during 2022-2023.
- Economic activity remained surprisingly resilient.
- Global inflation direction is distinct from country-level inflation rates.
- Resilient activity is not the same as accelerated growth everywhere.
- Mid-2022 peak is distinct from annual-average inflation.
- The statement is a narrative summary, not a forecast-table value.

### Expected Response Sections

- Conclusion describing falling inflation and resilient activity.
- Source comparison anchored in the official macroeconomic outlook.
- Boundary explanation about global/country scope, disinflation/deflation, and resilience/growth acceleration.
- Caveat about narrative scope and source period.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes inflation direction, activity resilience, period/peak, evidence, caveat, and confidence.
- 1: Includes inflation direction but weakly covers activity or period.
- 0: Does not answer the disinflation/resilience narrative.

**Accuracy**
- 2: States inflation descended from mid-2022 peak while activity remained resilient during 2022-2023.
- 1: Gives a broadly correct narrative but omits mid-2022 or resilience detail.
- 0: Describes deflation, a single country, or universal growth acceleration.

**Reasoning**
- 2: Distinguishes global/country inflation, resilience/acceleration, mid-2022 peak/annual average, and narrative/forecast table.
- 1: Mentions one boundary but leaves interpretation unclear.
- 0: Conflates disinflation with deflation or country rates.

**Use of Evidence**
- 2: Uses official outlook evidence and corroborates only compatible macro summary context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported macro commentary.

**Clarity and Structure**
- 2: Clear concise narrative answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing macroeconomic summary.

### Common Failure Modes

- Saying activity accelerated everywhere.
- Reporting a single country's inflation rate.
- Treating the disinflation narrative as deflation.
- Omitting either inflation direction or activity resilience.

### Borderline Cases

- "Inflation eased" is acceptable for descended.
- Do not require numeric inflation rates.
- Country examples are acceptable only as context, not the answer.

---

## 3. CORE-ECON-19

rubric_id: CORE-RUBRIC-B09-CORE-ECON-19
task_type: Core
research_object: emerging-market foreign-direct-investment outlook
answer_unit: expected direction of FDI flows and policy condition for reinvigoration

### Key Facts From Source Bundle

- FDI flows to emerging-market and developing economies are likely to weaken.
- The weakening is linked to uncertainty and growing protectionism.
- Reinvigorating FDI requires improving institutions.
- Reinvigorating FDI also requires safeguarding policy stability.
- FDI flows are distinct from portfolio flows.
- Expected weakening is distinct from an observed historical decline.
- The aggregate outlook is distinct from individual-country cases.

### Expected Response Sections

- Conclusion with expected FDI weakening and policy conditions.
- Source comparison anchored in the official analytical source.
- Boundary explanation about FDI/portfolio flows, expected/observed status, and aggregate/country scope.
- Caveat about uncertainty, protectionism, and policy conditions.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes direction, uncertainty/protectionism, institution/policy-stability conditions, evidence, caveat, and confidence.
- 1: Gives direction but omits one policy condition or caveat.
- 0: Does not answer FDI outlook.

**Accuracy**
- 2: States likely weakening of EMDE FDI and need to improve institutions and safeguard policy stability.
- 1: Gives weakening and one condition.
- 0: Reports portfolio flows or says stimulus alone reinvigorates FDI.

**Reasoning**
- 2: Distinguishes FDI/portfolio flows, expected weakening/observed decline, policy stability/stimulus, and aggregate/country cases.
- 1: Mentions one boundary but leaves source scope unclear.
- 0: Treats the outlook as observed for every country.

**Use of Evidence**
- 2: Uses official analytical evidence and corroborates only compatible FDI/policy context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic investment commentary.

**Clarity and Structure**
- 2: Clear outlook-plus-condition answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Unfocused investment discussion.

### Common Failure Modes

- Reporting portfolio investment instead of FDI.
- Treating the outlook as already observed for every country.
- Omitting the institutional/policy-stability condition.
- Saying stimulus alone reinvigorates FDI.

### Borderline Cases

- "Emerging markets and developing economies" and "EMDEs" are equivalent.
- Do not require country examples.
- If later FDI data are mentioned, they must be separated from the outlook statement.

---

## 4. CORE-ECON-09

rubric_id: CORE-RUBRIC-B09-CORE-ECON-09
task_type: Core
research_object: insurance group AI deployment statement
answer_unit: number of AI applications and tools in deployment and development

### Key Facts From Source Bundle

- The insurance group's AI specialists, engineers, scientists, and developers have **over 500 AI applications and tools**.
- These applications and tools are in deployment and development.
- Applications/tools are distinct from employees or models.
- Deployed tools are distinct from tools still in development.
- The statement is an internal capability statement, not necessarily an audited KPI.
- Current-year company report text should not be replaced by later public claims without caveat.

### Expected Response Sections

- Conclusion with the over-500 applications/tools figure.
- Source comparison anchored in the official company report.
- Boundary explanation about deployment/development, applications/tools, and capability statement status.
- Caveat about KPI/audit status and later updates.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes over-500 count, deployment/development status, object type, evidence, caveat, and confidence.
- 1: Gives count but omits deployment/development or caveat.
- 0: Does not answer the AI applications/tools question.

**Accuracy**
- 2: Reports **over 500 AI applications and tools in deployment and development**.
- 1: Reports 500+ but labels scope imprecisely.
- 0: Reports number of staff, models, or fully deployed tools only.

**Reasoning**
- 2: Distinguishes deployed/development, applications-tools/employees-models, internal capability/audited KPI, and current report/later claims.
- 1: Mentions one boundary but leaves status unclear.
- 0: Treats the statement as externally verified performance evidence.

**Use of Evidence**
- 2: Uses official company report evidence and corroborates only compatible current-year updates.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported AI marketing claims.

**Clarity and Structure**
- 2: Clear count-and-scope answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing AI deployment answer.

### Common Failure Modes

- Reporting number of staff instead of applications/tools.
- Treating all 500+ tools as fully deployed.
- Omitting "over" or "in deployment and development."
- Treating the statement as externally verified performance evidence.

### Borderline Cases

- "More than 500" is acceptable.
- Do not require a list of applications.
- Later public claims should be caveated as updates.

---

## 5. BND-CORE-PAIR-031

rubric_id: CORE-RUBRIC-B09-BND-CORE-PAIR-031
task_type: Core
research_object: 2024 internal-audit report inclusion exception
answer_unit: audit report issue date and reason it was included in the 2024 annual report

### Key Facts From Source Bundle

- The final audit report was issued on **10 March 2025**.
- It was exceptionally included in the **2024** Annual Internal Audit report.
- The reason for inclusion was that audit work was completed in 2024.
- Audit work timing is distinct from final report issuance.
- Exceptional inclusion is distinct from regular reporting scope.
- Annual report year is distinct from audit issue date.

### Expected Response Sections

- Conclusion with issue date and reason for 2024 inclusion.
- Source comparison anchored in the official audit report.
- Boundary explanation about work completion, issue date, annual-report year, and exception status.
- Caveat about audit area and reporting scope.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes date, 2024 inclusion, reason, evidence, caveat, and confidence.
- 1: Includes date and inclusion but omits reason or caveat.
- 0: Does not answer inclusion exception.

**Accuracy**
- 2: States **10 March 2025** issue date and inclusion in 2024 report because audit work was completed in 2024.
- 1: Gets date or reason correct but not both.
- 0: Says the report was issued in 2024 or omits the exception.

**Reasoning**
- 2: Distinguishes audit work/report issuance, exceptional/regular scope, annual-report year/issue date, and audit area/all audit activity.
- 1: Mentions one boundary but leaves exception unclear.
- 0: Treats the exception as normal reporting practice.

**Use of Evidence**
- 2: Uses official audit-report evidence and corroborates only compatible reporting-scope details.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported audit summaries.

**Clarity and Structure**
- 2: Clear date-plus-reason answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing audit-report answer.

### Common Failure Modes

- Saying the report was issued in 2024.
- Treating the exception as normal reporting practice.
- Omitting the reason for inclusion.
- Confusing audit area with all capital-market activity.

### Borderline Cases

- If audit area is omitted, score can still be high if date and reason are precise.
- Do not require naming every audit recommendation.
- "Finalised" should be checked against whether it means work completed or report issued.

---

## 6. CORE-ECON-22

rubric_id: CORE-RUBRIC-B09-CORE-ECON-22
task_type: Core
research_object: public-spending efficiency evidence base
answer_unit: country coverage and time window for efficiency scores

### Key Facts From Source Bundle

- Average efficiency scores are derived from up to **five methodologies**.
- Scores cover up to **146 emerging-market and developing economies**.
- Sectors are health, education, and infrastructure spending.
- The evidence window is **2010-2020**.
- Efficiency scores are distinct from spending levels.
- "Up to" coverage should not be converted into complete coverage for all methods.
- The evidence window is distinct from current fiscal projections.

### Expected Response Sections

- Conclusion with methods, country coverage, sectors, and time window.
- Source comparison anchored in the official analytical source.
- Boundary explanation about scores/spending, up-to coverage, sectors, and evidence/projection timing.
- Caveat about methodological coverage.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes methods, countries, sectors, time window, evidence, caveat, and confidence.
- 1: Includes country/time coverage but omits methods or sectors.
- 0: Does not answer evidence-base coverage.

**Accuracy**
- 2: Reports up to **five methodologies**, up to **146 EMDEs**, health/education/infrastructure, **2010-2020**.
- 1: Gets most components but omits "up to" or sectors.
- 0: Treats 146 as full coverage for every method or reports spending amounts.

**Reasoning**
- 2: Distinguishes efficiency scores/spending levels, up-to/full coverage, sector-specific/total spending, and evidence window/current projections.
- 1: Mentions one boundary but leaves coverage unclear.
- 0: Uses current-year projections as the evidence base.

**Use of Evidence**
- 2: Uses official figure-note/source evidence and corroborates only compatible methodology context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated fiscal-efficiency claims.

**Clarity and Structure**
- 2: Clear coverage/time-window answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing fiscal-efficiency response.

### Common Failure Modes

- Reporting 146 as full coverage for every methodology.
- Treating scores as spending amounts.
- Omitting sectors or time window.
- Using current-year projections as the evidence base.

### Borderline Cases

- "As many as 146" is acceptable for "up to 146."
- Do not require naming all five methodologies.
- Partial credit if sectors are summarized as social and infrastructure spending but not fully named.

---

## 7. BND-CORE-PAIR-051

rubric_id: CORE-RUBRIC-B09-BND-CORE-PAIR-051
task_type: Core
research_object: high-value-dataset reuse monitoring status
answer_unit: whether activities or incentives exist to monitor and measure reuse

### Key Facts From Source Bundle

- The country response records **No** for activities or incentives to monitor and measure reuse of high-value datasets.
- High-value-dataset reuse is distinct from general open-data reuse.
- Activities/incentives are distinct from passive portal availability.
- Monitoring status is distinct from examples of reuse cases.
- Questionnaire status may differ from later implementation changes.
- Related non-open-data inventory rows should not be used to infer beyond the boundary.

### Expected Response Sections

- Conclusion with the "No" status.
- Source comparison anchored in the official country response.
- Boundary explanation about high-value datasets, monitoring/incentives, portal availability, and reuse examples.
- Caveat about questionnaire date and later implementation.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes No status, high-value-dataset scope, monitoring/incentive boundary, evidence, caveat, and confidence.
- 1: Gives No but omits scope or caveat.
- 0: Does not answer reuse-monitoring status.

**Accuracy**
- 2: Reports **No** activities or incentives to monitor/measure high-value-dataset reuse.
- 1: Gives No but labels it as general open-data reuse.
- 0: Reports reuse examples as monitoring incentives or ignores explicit No.

**Reasoning**
- 2: Distinguishes HVD/general reuse, activities-incentives/passive availability, monitoring/reuse cases, and questionnaire/later status.
- 1: Mentions one boundary but leaves status scope unclear.
- 0: Treats portal availability as reuse measurement.

**Use of Evidence**
- 2: Uses official country-response rows and corroborates only compatible status/update context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic high-value-dataset policy material.

**Clarity and Structure**
- 2: Clear No-status answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Ambiguous open-data response.

### Common Failure Modes

- Reporting reuse examples as monitoring incentives.
- Answering about all open data rather than high-value datasets.
- Ignoring the explicit "No" response.
- Treating portal availability as reuse measurement.

### Borderline Cases

- If later activities exist, they must be framed as updates to the questionnaire status.
- Do not require naming every HVD category.
- Related inventory rows should not change the monitoring answer.

---

## 8. BND-CORE-PAIR-026

rubric_id: CORE-RUBRIC-B09-BND-CORE-PAIR-026
task_type: Core
research_object: extreme-heat exposure wellbeing indicator
answer_unit: temperature threshold and minimum exposure duration

### Key Facts From Source Bundle

- Exposure to hot days is defined using maximum temperature above **35 degrees Celsius**.
- Exposure must last at least **two weeks a year**.
- The threshold is maximum daily temperature, not average temperature.
- Exposure duration is distinct from a single-day heat event.
- The indicator concerns wellbeing, not an emissions or climate target.
- Population exposure is distinct from geographic heat occurrence.

### Expected Response Sections

- Conclusion with the temperature threshold and exposure duration.
- Source comparison anchored in the official statistical/wellbeing source.
- Boundary explanation about maximum/average temperature, duration, wellbeing indicator, and population exposure.
- Caveat about indicator definition and measurement scope.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes 35C, two weeks/year, indicator scope, evidence, caveat, and confidence.
- 1: Gives threshold but omits duration or indicator scope.
- 0: Does not define exposure.

**Accuracy**
- 2: Defines exposure as maximum temperature above **35C** for at least **two weeks a year**.
- 1: Gives one component correctly.
- 0: Uses average temperature, one-day threshold, or emissions target.

**Reasoning**
- 2: Distinguishes maximum/average temperature, duration/single-day event, wellbeing indicator/climate target, and population/geographic exposure.
- 1: Mentions one boundary but leaves exposure definition unclear.
- 0: Treats geographic heat occurrence as population exposure.

**Use of Evidence**
- 2: Uses official statistical source evidence and corroborates only compatible indicator-definition context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic heatwave definitions.

**Clarity and Structure**
- 2: Clear definition with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing heat indicator response.

### Common Failure Modes

- Using average temperature instead of maximum temperature.
- Reporting a one-day heatwave threshold.
- Omitting the two-week duration.
- Treating the indicator as an emissions target.

### Borderline Cases

- "35 deg C" or "35°C" is acceptable.
- Do not require health-impact quantification.
- If local heatwave definitions differ, they should not replace the indicator definition.

---

## 9. BND-CORE-PAIR-055

rubric_id: CORE-RUBRIC-B09-BND-CORE-PAIR-055
task_type: Core
research_object: national data portal request-feature status
answer_unit: whether the portal enables dataset requests and monitors request-to-publication outcomes

### Key Facts From Source Bundle

- The country response records **No** for whether the portal enables users to request datasets through a request-data feature.
- It also records **No** for monitoring the extent to which requests result in publication of requested data.
- Contact forms are distinct from dataset-request buttons.
- Request enablement is distinct from request-to-publication monitoring.
- Portal functionality is distinct from off-portal processes.
- Questionnaire status may change after portal redesigns.

### Expected Response Sections

- Conclusion with both No statuses.
- Source comparison anchored in the official country response.
- Boundary explanation about request features, contact forms, monitoring, and portal/off-portal process.
- Caveat about questionnaire date and later redesigns.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes both No statuses, feature/monitoring boundary, evidence, caveat, and confidence.
- 1: Includes one status fully and the other partially.
- 0: Does not answer portal request-feature status.

**Accuracy**
- 2: Reports **No** request-data feature and **No** request-to-publication monitoring.
- 1: Gets one status correct or labels one imprecisely.
- 0: Treats a contact form as a request-data feature or claims monitoring without evidence.

**Reasoning**
- 2: Distinguishes contact forms/request buttons, enablement/monitoring, portal/off-portal processes, and questionnaire/redesign status.
- 1: Mentions one boundary but leaves feature status unclear.
- 0: Generalises from other portals.

**Use of Evidence**
- 2: Uses official country-response portal rows and corroborates only compatible portal-status context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic portal-function claims.

**Clarity and Structure**
- 2: Clear two-status answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Ambiguous portal-function response.

### Common Failure Modes

- Treating a contact form as a request-data feature.
- Saying request outcomes are monitored without evidence.
- Answering only one of the two statuses.
- Generalising from other national portals.

### Borderline Cases

- A table with the two statuses is acceptable.
- Later portal redesigns should be caveated separately.
- Off-portal request processes do not change portal-feature status unless source says so.

---

## 10. CORE-GEN-10

rubric_id: CORE-RUBRIC-B09-CORE-GEN-10
task_type: Core
research_object: public-integrity indicators approval timeline
answer_unit: approval year and participating working-party countries

### Key Facts From Source Bundle

- The public-integrity indicators were approved in **2019**.
- Approval was by all member countries.
- Participating working-party countries include Austria, Brazil, Chile, Czechia, Finland, France, Germany, Greece, Italy, the Netherlands, Poland, the Slovak Republic, the United Kingdom, and the United States.
- Approval by all member countries is distinct from working-party participation.
- Acknowledgement country list is distinct from full indicator coverage.
- Approval year is distinct from report publication year.
- Public-integrity indicators are distinct from open-data indicators.

### Expected Response Sections

- Conclusion with approval year and participation/approval distinction.
- Source comparison anchored in the official governance-indicators source.
- Boundary explanation about approval, working-party list, coverage, publication year, and framework type.
- Caveat about list role and indicator coverage.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes 2019 approval, all-member approval, working-party examples/list role, evidence, caveat, and confidence.
- 1: Includes approval year but weakly handles working-party distinction.
- 0: Does not answer approval timeline.

**Accuracy**
- 2: Reports **2019** approval by all member countries and correctly treats listed countries as participating working-party countries.
- 1: Gets 2019 but misstates list role partially.
- 0: Treats working-party list as all covered countries or gives publication year.

**Reasoning**
- 2: Distinguishes approval/participation, acknowledgement list/full coverage, approval/publication year, and public-integrity/open-data indicators.
- 1: Mentions one distinction but leaves approval scope unclear.
- 0: Confuses public-integrity and open-data frameworks.

**Use of Evidence**
- 2: Uses official governance-indicators evidence and corroborates only compatible methodology/acknowledgement context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated integrity/open-data sources.

**Clarity and Structure**
- 2: Clear timeline-plus-list-role answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing indicators answer.

### Common Failure Modes

- Treating the working-party list as all covered countries.
- Reporting publication year instead of approval year.
- Omitting the approval-by-member-countries distinction.
- Confusing public-integrity and open-data frameworks.

### Borderline Cases

- The full working-party list need not be exhaustive if enough examples are given and list role is clear.
- Do not require country coverage of every indicator.
- "Czech Republic" may be acceptable for Czechia if source-compatible.

---

## 11. CORE-ECON-21

rubric_id: CORE-RUBRIC-B09-CORE-ECON-21
task_type: Core
research_object: Lebanon 2024 conflict economic contraction estimate
answer_unit: expected real GDP contraction with and without conflict scenario

### Key Facts From Source Bundle

- Activity is expected to contract by **5.7% in 2024**.
- Under a no-conflict scenario, activity would have grown by **0.9%**.
- A related real GDP contraction reference is **6.6%** where relevant.
- Expected/observed contraction is distinct from counterfactual no-conflict growth.
- Real GDP is distinct from nominal activity.
- Conflict-specific impact is distinct from broader crisis baseline.
- Arabic summaries and translated tables must be reconciled carefully if both are used.

### Expected Response Sections

- Conclusion with the conflict contraction and no-conflict scenario.
- Source comparison anchored in the official country economic source.
- Boundary explanation about actual/counterfactual, real/nominal, conflict/broader baseline, and translated-source reconciliation.
- Caveat about scenario and source-language/table differences.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes 5.7% contraction, 0.9% no-conflict growth, 6.6% reference if used, evidence, caveat, and confidence.
- 1: Includes contraction and scenario but omits caveat or 6.6% context.
- 0: Does not answer contraction with/without conflict.

**Accuracy**
- 2: Reports **5.7% contraction** versus **0.9% no-conflict growth**, with **6.6% real GDP contraction** handled as related context where relevant.
- 1: Gets main contraction or scenario correct but not both.
- 0: Treats 0.9% as actual growth or reports nominal measures.

**Reasoning**
- 2: Distinguishes actual/counterfactual, real/nominal, conflict-specific/broader crisis, and Arabic/translated table figures.
- 1: Mentions one boundary but leaves scenario unclear.
- 0: Reports only no-conflict scenario or mixes measures.

**Use of Evidence**
- 2: Uses official country economic source and corroborates only compatible scenario/source-language details.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported conflict-economic claims.

**Clarity and Structure**
- 2: Clear scenario comparison with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing Lebanon macro answer.

### Common Failure Modes

- Reporting only the no-conflict scenario.
- Treating 0.9% as actual growth.
- Omitting the contraction value.
- Mixing nominal and real GDP measures.

### Borderline Cases

- If the answer gives both 5.7% and 6.6%, it must explain the source distinction.
- Do not require detailed conflict chronology.
- "Activity" is acceptable if tied to real GDP/source wording.

---

## 12. BND-CORE-PAIR-037

rubric_id: CORE-RUBRIC-B09-BND-CORE-PAIR-037
task_type: Core
research_object: renewable-generation forecasting reuse case
answer_unit: estimated balancing-cost reduction and solar-generation trend

### Key Facts From Source Bundle

- Forecasting services helped generators reduce balancing-energy costs by **5-7%** in recent years.
- Solar energy generated is increasing by almost **10% year on year**.
- Balancing-energy cost reduction is distinct from total generation cost.
- Forecasting-service contribution is distinct from scheme-wide causality.
- Solar-generation growth is distinct from installed-capacity growth.
- Open meteorological data are distinct from proprietary forecasting methods.

### Expected Response Sections

- Conclusion with cost-reduction range and solar-generation trend.
- Source comparison anchored in the official country response.
- Boundary explanation about balancing costs, causality, generation/capacity, and open/proprietary data.
- Caveat about reuse-case evidence and causality.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes 5-7%, almost 10% YoY, boundaries, evidence, caveat, and confidence.
- 1: Includes one figure fully and the other partially.
- 0: Does not answer forecasting reuse case.

**Accuracy**
- 2: Reports **5-7%** balancing-cost reduction and solar generation increasing almost **10% year on year**.
- 1: Gets one metric correct or labels one imprecisely.
- 0: Applies 5-7% to all energy costs or reports capacity growth.

**Reasoning**
- 2: Distinguishes balancing/total costs, contribution/causality, generation/capacity, and open meteorological/proprietary forecasting.
- 1: Mentions one boundary but leaves causal interpretation unclear.
- 0: Treats forecasting as sole cause of scheme success.

**Use of Evidence**
- 2: Uses official country-response evidence and corroborates only compatible renewable-generation context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated energy-market claims.

**Clarity and Structure**
- 2: Clear two-metric answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing renewable-generation answer.

### Common Failure Modes

- Applying 5-7% to all energy costs.
- Treating the forecasting service as the sole cause of the whole scheme's success.
- Reporting solar capacity rather than generation.
- Omitting the year-on-year qualifier.

### Borderline Cases

- "Five to seven percent" and "nearly 10%" are acceptable.
- Do not require proof of full causal attribution.
- If installed capacity is mentioned, generation trend must remain primary.

---

## 13. CORE-POL-32

rubric_id: CORE-RUBRIC-B09-CORE-POL-32
task_type: Core
research_object: open-data real-estate estimation reuse case
answer_unit: purpose of the tool and market-context caveat

### Key Facts From Source Bundle

- The reuse case is a real-estate value estimation tool.
- The tool provides indicative value estimation, not official appraisal.
- The context is a crisis in real-estate sales.
- Such tools are useful indicators of data relevance.
- Reuse-case relevance is distinct from measured market impact.
- Real-estate sales crisis context is distinct from tool accuracy.
- Open-data use is distinct from private model assumptions.

### Expected Response Sections

- Conclusion with tool purpose and market-context caveat.
- Source comparison anchored in the official country response.
- Boundary explanation about indicative valuation, appraisal, market impact, and model assumptions.
- Caveat about crisis context and evidence limits.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes tool purpose, crisis context, data-relevance caveat, evidence, caveat, and confidence.
- 1: Includes tool purpose but weakly handles market context.
- 0: Does not answer the reuse-case purpose.

**Accuracy**
- 2: Describes an indicative real-estate value estimation tool useful as a data-relevance indicator during a sales crisis, not proof of market impact/appraisal accuracy.
- 1: Describes valuation tool but omits one boundary.
- 0: Treats the tool as official valuation or measured market impact.

**Reasoning**
- 2: Distinguishes indicative valuation/appraisal, reuse relevance/market impact, crisis context/tool accuracy, and open data/private model assumptions.
- 1: Mentions one boundary but leaves reliability unclear.
- 0: Claims unsupported appraisal accuracy or impact.

**Use of Evidence**
- 2: Uses official country-response evidence and corroborates only compatible reuse-case context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic real-estate model claims.

**Clarity and Structure**
- 2: Clear purpose-plus-caveat answer with confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing real-estate reuse answer.

### Common Failure Modes

- Treating the tool as an official valuation.
- Claiming measured market impact without evidence.
- Omitting the real-estate sales crisis caveat.
- Ignoring private model assumptions.

### Borderline Cases

- "Indicative estimate" is acceptable for value estimation.
- Do not require naming the tool.
- Market context should not be used to infer accuracy.

---

## 14. CORE-ECON-04

rubric_id: CORE-RUBRIC-B09-CORE-ECON-04
task_type: Core
research_object: shipping-price shock simulation
answer_unit: assumed first-quarter price increase and persistence over the simulation horizon

### Key Facts From Source Bundle

- The simulation assumes shipping prices rise by **100% in the first quarter**.
- Shipping prices remain permanently higher throughout the whole simulation horizon.
- The assumption is distinct from observed freight rates.
- First-quarter shock is distinct from annual average change.
- Permanently higher level is distinct from continued growth every period.
- Simulation horizon is distinct from forecast publication date.

### Expected Response Sections

- Conclusion with the first-quarter 100% shock and persistence assumption.
- Source comparison anchored in the official macroeconomic simulation source.
- Boundary explanation about assumption/observed data, first-quarter/annual change, level/growth, and horizon/publication date.
- Caveat about simulation status.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes 100%, first quarter, permanent higher level, evidence, caveat, and confidence.
- 1: Includes shock but omits persistence or simulation caveat.
- 0: Does not answer shipping-price simulation assumption.

**Accuracy**
- 2: States **100% first-quarter increase** and prices remain permanently higher over the horizon.
- 1: Gets one component correct.
- 0: Treats the 100% increase as observed data or says prices double every quarter.

**Reasoning**
- 2: Distinguishes assumption/observed rates, first-quarter/annual average, permanent level/continued growth, and simulation horizon/publication date.
- 1: Mentions one boundary but leaves persistence unclear.
- 0: Reports annual shipping inflation or repeated quarterly doubling.

**Use of Evidence**
- 2: Uses official simulation evidence and corroborates only compatible scenario details.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated freight-rate data as the simulation assumption.

**Clarity and Structure**
- 2: Clear simulation-assumption answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing shipping-price answer.

### Common Failure Modes

- Treating the 100% increase as observed data.
- Saying prices keep doubling every quarter.
- Reporting annual average shipping inflation.
- Omitting persistence over the horizon.

### Borderline Cases

- "Prices double in Q1" is acceptable if it is explicitly a simulation assumption.
- Do not require the full model horizon length if not in source.
- Observed freight data may be used only as context.

---

## 15. BND-CORE-PAIR-033

rubric_id: CORE-RUBRIC-B09-BND-CORE-PAIR-033
task_type: Core
research_object: data-protection fine in energy-efficiency programme case
answer_unit: fine amount and court outcome

### Key Facts From Source Bundle

- The authority levied a fine of **HUF 110 million**.
- The approximate euro amount is **EUR 275,000**.
- The authority won the subsequent court case.
- The court fully approved the decision.
- Local-currency fine is distinct from euro approximation.
- Authority decision is distinct from court approval.
- The case must be kept separate from other data-protection cases in the report.

### Expected Response Sections

- Conclusion with fine amount and court outcome.
- Source comparison anchored in the official data-protection case source.
- Boundary explanation about currency, authority/court decisions, controller/processor if relevant, and case identity.
- Caveat about approximation and case scope.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes HUF fine, EUR approximation, court outcome, evidence, caveat, and confidence.
- 1: Includes fine and court outcome but omits one currency or caveat.
- 0: Does not answer fine/court outcome.

**Accuracy**
- 2: Reports **HUF 110 million**, approximately **EUR 275,000**, and court fully approved the authority's decision.
- 1: Gets amount or court outcome partially correct.
- 0: Says court overturned the decision or mixes another case.

**Reasoning**
- 2: Distinguishes local/euro amounts, authority decision/court approval, controller/processor where relevant, and this case/other cases.
- 1: Mentions one boundary but leaves case status unclear.
- 0: Treats euro approximation as the sole exact fine or wrong case.

**Use of Evidence**
- 2: Uses official data-protection case evidence and corroborates only compatible case/status details.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated fine databases or cases.

**Clarity and Structure**
- 2: Clear legal/status answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing data-protection case answer.

### Common Failure Modes

- Reporting only the euro approximation.
- Saying the court overturned the decision.
- Mixing this case with another fine in the report.
- Omitting the court outcome.

### Borderline Cases

- "Forint" is acceptable for HUF.
- Do not require detailed court reasoning.
- Currency conversion should be caveated as approximate.

---

## 16. CORE-TECH-10

rubric_id: CORE-RUBRIC-B09-CORE-TECH-10
task_type: Core
research_object: AI risk-measurement process evaluation
answer_unit: requirement to evaluate and document deployed metrics and processes

### Key Facts From Source Bundle

- Deployed testing, evaluation, validation, and verification metrics are evaluated and documented.
- Deployed testing, evaluation, validation, and verification processes are evaluated and documented.
- Mechanisms for tracking identified AI risks over time are in place.
- Deployed metrics are distinct from proposed metrics.
- Evaluation is distinct from one-time validation.
- Documentation is distinct from public disclosure.
- Risk-measurement process is distinct from risk-mapping or risk-management functions.

### Expected Response Sections

- Conclusion with evaluation/documentation requirement and risk-tracking mechanism.
- Source comparison anchored in the controlling framework source.
- Boundary explanation about deployed/proposed metrics, evaluation/validation, documentation/disclosure, and measurement/mapping/management.
- Caveat about framework status and implementation context.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes deployed TEVV metrics/processes, evaluation, documentation, risk tracking, evidence, caveat, and confidence.
- 1: Includes evaluation/documentation but omits risk tracking or deployed status.
- 0: Does not answer risk-measurement process evaluation.

**Accuracy**
- 2: States deployed TEVV metrics/processes are evaluated and documented and risks are tracked over time.
- 1: Gives a partial process requirement but omits one element.
- 0: Discusses risk mapping instead or reports proposed metrics as deployed.

**Reasoning**
- 2: Distinguishes deployed/proposed metrics, evaluation/one-time validation, documentation/disclosure, and risk measurement/mapping/management.
- 1: Mentions one boundary but leaves process status unclear.
- 0: Treats documentation as public transparency by default.

**Use of Evidence**
- 2: Uses controlling framework evidence and corroborates only compatible measurement-function details.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic AI risk-management advice.

**Clarity and Structure**
- 2: Clear framework-process answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing AI-risk answer.

### Common Failure Modes

- Discussing risk mapping instead of measurement-process evaluation.
- Treating documentation as public transparency by default.
- Omitting tracking of identified risks over time.
- Reporting proposed metrics rather than deployed ones.

### Borderline Cases

- "TEVV" is acceptable if expanded or clearly tied to testing/evaluation/validation/verification.
- Do not require public disclosure details.
- Legal-duty claims should be caveated unless source supports them.
