# Manual Deep-Research Prompt Batch 009

Runnable benchmark items only. This file uses the final hybrid deep-research benchmark method: each prompt keeps one research object and one answer target, but requires source comparison, boundary/methodology judgement, discrepancy handling, and confidence rather than a single-fact lookup.

Mandatory rule:
- Core = one object + one disputed or methodology-sensitive parameter + one trap about definitions, dates, reporting scope, update status, or source comparability.
- Set = one explicit `candidate_item` + one real boundary condition; the prompt must not merely ask whether the item appears in a list.
- Use the official primary source as the anchor, and at least one corroborating secondary source where available. If one primary register, legal act, official table, or underlying study is controlling, explain why and use other sources only to check revisions, naming, boundary conflicts, or later summaries.
- Answer format: conclusion, source comparison, caveat, and confidence level.
- Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond that boundary.
- Include a trend or update signal only when the source context makes time change relevant.
- Do not ask for broad list retrieval or an essay unrelated to the named research object.

---

## 1. BND-CORE-PAIR-005

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: restricted-stock-unit vesting schedule
answer_unit: first-anniversary vesting share and later vesting share

source_anchor:
- Equity-plan text says time-based vesting allows 25% of units awarded to vest on the first anniversary of employment.
- It says the remaining 75% are subsequently eligible to vest over the rest of the four-year period.

internal_source_boundary:
- source_name: internal equity-compensation source bundle
- source_scope: time-based vesting paragraph for restricted stock units and related award terms

final_prompt_text:
Use the official company award document as anchor and one corroborating source if available. For restricted-stock-unit vesting schedule, resolve first-anniversary vesting share and later vesting share.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish time-based vesting from performance awards, first-anniversary eligibility from grant-date ownership, percentage of units from dollar value, and standard schedule from termination or special-award exceptions. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 2. BND-CORE-PAIR-009

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: global disinflation resilience narrative
answer_unit: direction of inflation and activity during 2022-2023

source_anchor:
- Economic outlook text says economic activity was surprisingly resilient through the global disinflation of 2022-2023.
- It says global inflation descended from its mid-2022 peak while activity remained resilient.

internal_source_boundary:
- source_name: internal global economic outlook source bundle
- source_scope: opening summary paragraph on global disinflation, inflation peak, and economic activity resilience

final_prompt_text:
Use the official macroeconomic outlook as anchor and one corroborating source if available. For global disinflation resilience narrative, resolve the direction of inflation and activity during 2022-2023.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish global inflation direction from country-level inflation rates, resilience of activity from acceleration of growth, mid-2022 peak from annual-average inflation, and narrative summary from forecast tables. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 3. CORE-ECON-19

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: emerging-market foreign-direct-investment outlook
answer_unit: expected direction of FDI flows and policy condition for reinvigoration

source_anchor:
- Development-economics text says FDI flows to emerging-market and developing economies will likely weaken amid uncertainty and growing protectionism.
- It says reinvigorating FDI requires improving institutions and safeguarding policy stability.

internal_source_boundary:
- source_name: internal development-economics source bundle
- source_scope: paragraph on FDI flows, uncertainty, protectionism, technology diffusion, institutional improvement, and policy stability

final_prompt_text:
Use the official analytical source as anchor and one corroborating source if available. For emerging-market foreign-direct-investment outlook, resolve expected direction of FDI flows and policy condition for reinvigoration.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish FDI flows from portfolio flows, expected weakening from observed historical decline, policy stability from short-term stimulus, and emerging-market aggregate from individual-country cases. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 4. CORE-ECON-09

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: insurance group AI deployment statement
answer_unit: number of AI applications and tools in deployment and development

source_anchor:
- Annual-report text says the company's AI specialists, engineers, scientists, and developers have over 500 AI applications and tools in deployment and development.

internal_source_boundary:
- source_name: internal insurance-group annual-report source bundle
- source_scope: AI capability paragraph naming internal AI team and number of applications/tools in deployment and development

final_prompt_text:
Use the official company report as anchor and one corroborating source if available. For insurance group AI deployment statement, resolve number of AI applications and tools in deployment and development.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish deployed tools from tools in development, applications from employees or models, internal capability statement from audited KPI, and current-year report text from later public claims. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 5. BND-CORE-PAIR-031

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: 2024 internal-audit report inclusion exception
answer_unit: audit report issue date and reason it was included in the 2024 annual report

source_anchor:
- Audit-report text says a final audit report for financial services and capital markets was issued on 10 March 2025.
- It says the audit is exceptionally included in the Annual Internal Audit report for 2024.

internal_source_boundary:
- source_name: internal annual internal-audit report source bundle
- source_scope: note on audit work completed in 2024, final report issued on 10 March 2025, and exceptional inclusion in 2024 annual reporting

final_prompt_text:
Use the official audit report as anchor and one corroborating source if available. For 2024 internal-audit report inclusion exception, resolve audit report issue date and reason it was included in the 2024 annual report.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish audit work performed in 2024 from final report issuance in 2025, exceptional inclusion from regular reporting scope, annual report year from audit issue date, and audit area from all internal-audit activity. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 6. CORE-ECON-22

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: public-spending efficiency evidence base
answer_unit: country coverage and time window for efficiency scores

source_anchor:
- Fiscal-policy figure note says average efficiency scores are derived from up to five methodologies.
- It says the scores cover up to 146 emerging-market and developing economies for health, education, and infrastructure spending over 2010-2020.

internal_source_boundary:
- source_name: internal fiscal-policy source bundle
- source_scope: figure note on public-spending efficiency scores, methodologies, country coverage, sectors, and 2010-2020 period

final_prompt_text:
Use the official analytical source as anchor and one corroborating source if available. For public-spending efficiency evidence base, resolve country coverage and time window for efficiency scores.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish efficiency scores from spending levels, "up to" country coverage from complete coverage, health/education/infrastructure spending from total public expenditure, and 2010-2020 evidence from current-year fiscal projections. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 7. BND-CORE-PAIR-051

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: high-value-dataset reuse monitoring status
answer_unit: whether activities or incentives exist to monitor and measure reuse

source_anchor:
- Country-response text records "no" for whether activities or incentives exist to monitor and measure reuse of high-value datasets.
- A related row also records "no" for whether inventories include non-open data collected by public bodies.

internal_source_boundary:
- source_name: internal open-data questionnaire source bundle
- source_scope: country response rows on high-value-dataset reuse monitoring incentives and non-open-data inventory coverage

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For high-value-dataset reuse monitoring status, resolve whether activities or incentives exist to monitor and measure reuse.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish high-value-dataset reuse from general open-data reuse, activities or incentives from passive portal availability, monitoring status from examples of reuse cases, and questionnaire answer from later implementation changes. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 8. BND-CORE-PAIR-026

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: extreme-heat exposure wellbeing indicator
answer_unit: temperature threshold and minimum exposure duration

source_anchor:
- Wellbeing-indicator text defines exposure to hot days as maximum temperature above 35 degrees Celsius for at least two weeks a year.
- It links the indicator to documented impacts on health and other wellbeing outcomes.

internal_source_boundary:
- source_name: internal wellbeing-indicator source bundle
- source_scope: extreme-temperature indicator note defining hot-day threshold, duration, and wellbeing relevance

final_prompt_text:
Use the official statistical source as anchor and one corroborating source if available. For extreme-heat exposure wellbeing indicator, resolve temperature threshold and minimum exposure duration.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish maximum daily temperature threshold from average temperature, exposure duration from single-day heat events, wellbeing indicator from climate target, and population exposure from geographic heat occurrence. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 9. BND-CORE-PAIR-055

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: national data portal request-feature status
answer_unit: whether the portal enables dataset requests and monitors request-to-publication outcomes

source_anchor:
- Country-response text records "No" for whether the national portal enables users to request datasets through a request-data feature.
- It also records "No" for whether the team monitors the extent to which requests result in publication of requested data.

internal_source_boundary:
- source_name: internal open-data portal questionnaire source bundle
- source_scope: portal feature rows on dataset request functionality and monitoring of request-to-publication outcomes

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For national data portal request-feature status, resolve whether the portal enables dataset requests and monitors request-to-publication outcomes.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish contact forms from dataset request buttons, request enablement from publication monitoring, portal functionality from off-portal processes, and questionnaire status from later portal redesigns. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 10. CORE-GEN-10

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: public-integrity indicators approval timeline
answer_unit: approval year and participating working-party countries

source_anchor:
- Governance-indicators text says the indicators were approved in 2019 by all member countries.
- It lists participating working-party countries including Austria, Brazil, Chile, Czechia, Finland, France, Germany, Greece, Italy, the Netherlands, Poland, the Slovak Republic, the United Kingdom, and the United States.

internal_source_boundary:
- source_name: internal public-integrity indicators source bundle
- source_scope: methodology/acknowledgement paragraph listing working-party countries and approval year

final_prompt_text:
Use the official governance-indicators source as anchor and one corroborating source if available. For public-integrity indicators approval timeline, resolve approval year and participating working-party countries.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish approval by member countries from working-party participation, country list in acknowledgements from full indicator coverage, approval year from report publication year, and public-integrity indicators from open-data indicators. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 11. CORE-ECON-21

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Lebanon 2024 conflict economic contraction estimate
answer_unit: expected real GDP contraction with and without conflict scenario

source_anchor:
- Country-economic text says activity is expected to contract by 5.7% in 2024 compared with 0.9% growth under a no-conflict scenario.
- It also references an estimated real GDP contraction of 6.6%.

internal_source_boundary:
- source_name: internal country economic update source bundle
- source_scope: Lebanon conflict-impact paragraph with 2024 contraction estimate, no-conflict scenario, and real GDP reference

final_prompt_text:
Use the official country economic source as anchor and one corroborating source if available. For Lebanon 2024 conflict economic contraction estimate, resolve expected real GDP contraction with and without conflict scenario.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish observed contraction from counterfactual no-conflict growth, real GDP from nominal activity, conflict-specific impact from broader crisis baseline, and Arabic summary figures from translated report tables. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 12. BND-CORE-PAIR-037

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: renewable-generation forecasting reuse case
answer_unit: estimated balancing-cost reduction and solar-generation trend

source_anchor:
- Country-response text says forecasting services helped generators reduce balancing-energy costs by 5-7% in recent years.
- It says this contributed to the success of the mandatory green power transfer scheme and that solar energy generated is increasing by almost 10% year on year.

internal_source_boundary:
- source_name: internal open-data reuse country-response source bundle
- source_scope: renewable-generation scheduling paragraph on meteorological data, forecasting companies, balancing-cost reduction, and solar-generation trend

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For renewable-generation forecasting reuse case, resolve estimated balancing-cost reduction and solar-generation trend.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish balancing-energy cost reduction from total generation cost, forecasting-service contribution from scheme-wide causality, solar-generation growth from installed capacity growth, and open meteorological data from proprietary forecasting methods. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 13. CORE-POL-32

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: open-data real-estate estimation reuse case
answer_unit: purpose of the tool and market-context caveat

source_anchor:
- Country-response text cites a real-estate value estimation tool as an open-data reuse case.
- It says that in difficult times marked by a crisis in real-estate sales, tools like this are a useful indicator of data relevance.

internal_source_boundary:
- source_name: internal open-data reuse country-response source bundle
- source_scope: paragraph on real-estate value estimation reuse case and real-estate sales crisis context

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For open-data real-estate estimation reuse case, resolve purpose of the tool and market-context caveat.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish indicative valuation from official appraisal, reuse-case relevance from measured market impact, real-estate sales crisis context from tool accuracy, and open-data use from private model assumptions. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 14. CORE-ECON-04

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: shipping-price shock simulation
answer_unit: assumed first-quarter price increase and persistence over the simulation horizon

source_anchor:
- Economic simulation note says shipping prices are assumed to rise by 100% in the first quarter.
- It says they remain permanently higher throughout the whole simulation horizon.

internal_source_boundary:
- source_name: internal macroeconomic simulation source bundle
- source_scope: simulation note on shipping-price assumption, first-quarter shock, and persistence over the horizon

final_prompt_text:
Use the official macroeconomic simulation source as anchor and one corroborating source if available. For shipping-price shock simulation, resolve assumed first-quarter price increase and persistence over the simulation horizon.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish shipping-price assumption from observed freight rates, first-quarter shock from annual average change, permanent higher level from continued growth, and simulation horizon from forecast publication date. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 15. BND-CORE-PAIR-033

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: data-protection fine in energy-efficiency programme case
answer_unit: fine amount and court outcome

source_anchor:
- Data-protection case text says the authority levied a fine of HUF 110 million, approximately EUR 275,000.
- It says the authority won the subsequent court case and the court fully approved the decision.

internal_source_boundary:
- source_name: internal data-protection annual-report source bundle
- source_scope: case paragraph on irregular processing in an energy-efficiency programme, fine amount, and court outcome

final_prompt_text:
Use the official data-protection case source as anchor and one corroborating source if available. For data-protection fine in energy-efficiency programme case, resolve fine amount and court outcome.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish local-currency fine from euro approximation, authority decision from court approval, data controller from data processor, and this energy-efficiency case from other data-protection cases in the report. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 16. CORE-TECH-10

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: AI risk-measurement process evaluation
answer_unit: requirement to evaluate and document deployed metrics and processes

source_anchor:
- AI risk-management text says deployed testing, evaluation, validation, and verification metrics and processes are evaluated and documented.
- It also says mechanisms for tracking identified AI risks over time are in place.

internal_source_boundary:
- source_name: internal AI risk-management framework source bundle
- source_scope: measurement-function rows on evaluating deployed TEVV metrics/processes and tracking identified AI risks over time

final_prompt_text:
Use the controlling framework source as anchor and one corroborating source if available. For AI risk-measurement process evaluation, resolve requirement to evaluate and document deployed metrics and processes.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish deployed metrics from proposed metrics, evaluation from one-time validation, documentation from public disclosure, and risk-measurement process from risk-mapping or risk-management functions. Return: current classification with boundary note, source comparison, caveat, and confidence.
