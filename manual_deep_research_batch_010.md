# Manual Deep-Research Prompt Batch 010

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

## 1. BND-CORE-PAIR-050

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: dynamic open-data publication constraints
answer_unit: allowed delay condition and temporary technical constraint

source_anchor:
- Open-data maturity text says countries with limited technical and financial capabilities may publish dynamic data within a longer time frame.
- It says this can include temporary technical constraints when immediate reuse availability is not feasible.

internal_source_boundary:
- source_name: internal open-data maturity source bundle
- source_scope: paragraph on dynamic-data publication, limited capabilities, longer time frames, and temporary technical constraints

final_prompt_text:
Use the official maturity-report source as anchor and one corroborating source if available. For dynamic open-data publication constraints, resolve allowed delay condition and temporary technical constraint.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish dynamic data from static datasets, delayed publication from exemption from publication, temporary technical constraints from permanent access limits, and policy guidance from a country-specific implementation claim. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 2. CORE-SCI-10

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: learning-poverty brief data-priority rule
answer_unit: hierarchy for school-age enrolment data and country data-year note

source_anchor:
- Learning-poverty methodology text says adjusted net enrolment rate is prioritised over total net enrolment rate and net enrolment rate for the year closest to the assessment year.
- It notes that one country brief uses 2022 data.

internal_source_boundary:
- source_name: internal learning-poverty country-brief source bundle
- source_scope: methodology note on enrolment-rate hierarchy, assessment-year proximity, and country-specific data-year note

final_prompt_text:
Use the official indicator brief as anchor and one corroborating source if available. For learning-poverty brief data-priority rule, resolve hierarchy for school-age enrolment data and the country data-year note.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish adjusted net enrolment from total net and net enrolment rates, data-year note from assessment year, school-age population denominator from total population, and country-specific footnote from general methodology. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 3. CORE-POL-16

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Latvia open-data quality controls in 2024
answer_unit: metadata-quality monitoring and quality-standard status

source_anchor:
- Country factsheet text records "Yes" for monitoring metadata quality on the portal.
- It also records "Yes" for setting standards on metadata quality.

internal_source_boundary:
- source_name: internal open-data maturity country-factsheet source bundle
- source_scope: Latvia factsheet quality-dimension key-question rows on metadata-quality monitoring and quality standards

final_prompt_text:
Use the official country factsheet as anchor and one corroborating source if available. For Latvia open-data quality controls in 2024, resolve metadata-quality monitoring and quality-standard status.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish metadata quality from dataset substantive quality, monitoring status from measured compliance, standards from legal mandates, and 2024 factsheet answers from later portal changes. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 4. BND-CORE-PAIR-030

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Spain national open-data action-plan additions by end-2023
answer_unit: action-plan complements and regional data-governance layer

source_anchor:
- Country response text says that by the end of 2023, the national open-data action plan was complemented by additional measures reflected on the national portal.
- It also cites regional data-governance models established by subnational governments.

internal_source_boundary:
- source_name: internal open-data strategy country-response source bundle
- source_scope: Spain response paragraphs on end-2023 action-plan complements, national portal reflection, and regional data-governance examples

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For Spain national open-data action-plan additions by end-2023, resolve action-plan complements and regional data-governance layer.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish national action-plan complements from regional governance models, end-2023 status from 2020-2024 strategy coverage, portal reflection from legal enactment, and open-data measures from broader data-governance policy. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 5. CORE-ECON-24

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: food-company 2027 cost-savings target
answer_unit: incremental savings target and timing

source_anchor:
- Company report text says the company aims to deliver incremental cost savings of at least CHF 2.5 billion by the end of 2027.
- It says these savings are on top of existing cost-savings programmes.

internal_source_boundary:
- source_name: internal company annual-report source bundle
- source_scope: performance and strategy paragraph on incremental cost savings, end-2027 timing, and relationship to existing programmes

final_prompt_text:
Use the official company report as anchor and one corroborating source if available. For food-company 2027 cost-savings target, resolve incremental savings target and timing.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish incremental savings from total cost base, target from realised savings, end-2027 timing from late-2024 announcement, and savings programme from revenue or margin guidance. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 6. BND-CORE-PAIR-036

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: worldwide governance indicator methodology coverage
answer_unit: economy coverage, time period, and source-count basis

source_anchor:
- Methodology paper text says aggregate governance indicators cover 214 economies over 1996-2023.
- It says the aggregate indicators combine information from 35 existing data sources.

internal_source_boundary:
- source_name: internal governance-indicator methodology source bundle
- source_scope: methodology introduction on economy sample, 1996-2023 period, aggregate indicators, and number of data sources

final_prompt_text:
Use the official methodology source as anchor and one corroborating source if available. For worldwide governance indicator methodology coverage, resolve economy coverage, time period, and source-count basis.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish economies from sovereign states, aggregate indicators from individual source measures, coverage period from publication year, and data-source count from number of governance dimensions. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 7. BND-CORE-PAIR-004

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: consumer-goods CEO departure terms in 2025
answer_unit: effective step-down date, leaving date, and leaver treatment

source_anchor:
- Annual-report text says the CEO stepped down as CEO and board director with effect from 1 March 2025 by mutual agreement.
- It says he will leave the company on 31 May 2025 and be treated as a good leaver for remuneration purposes.

internal_source_boundary:
- source_name: internal company annual-report source bundle
- source_scope: remuneration/governance paragraph on CEO step-down date, leaving date, mutual agreement, and good-leaver treatment

final_prompt_text:
Use the official company report as anchor and one corroborating source if available. For consumer-goods CEO departure terms in 2025, resolve effective step-down date, leaving date, and leaver treatment.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish stepping down from leaving employment, board-director role from CEO role, good-leaver treatment from severance amount, and mutual agreement from termination for cause. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 8. CORE-POL-19

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Poland geospatial open-data reuse support
answer_unit: educational resource and dataset-request process

source_anchor:
- Country factsheet text says the country maintains an educational geospatial website with e-learning resources and materials on geoportal and open-geodata applications.
- It says the portal administrator processes user requests for new datasets to encourage broader reuse and engagement.

internal_source_boundary:
- source_name: internal open-data maturity country-factsheet source bundle
- source_scope: Poland factsheet paragraph on geospatial education website, e-learning resources, geoportal materials, and user dataset requests

final_prompt_text:
Use the official country factsheet as anchor and one corroborating source if available. For Poland geospatial open-data reuse support, resolve educational resource and dataset-request process.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish geospatial education resources from portal maturity scores, user requests for new datasets from automatic publication, reuse encouragement from measured impact, and country-specific factsheet text from neighbouring country records. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 9. BND-CORE-PAIR-052

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: open-data air-quality notification reuse case
answer_unit: target users and pollution-season context

source_anchor:
- Country-response text describes an air-quality app that notifies users about air quality in their area.
- It says it is particularly useful in spring months with harmful high dust concentrations and for people with respiratory problems or outdoor workers.

internal_source_boundary:
- source_name: internal open-data reuse country-response source bundle
- source_scope: air-quality app reuse-case paragraph on spring dust concentrations, notifications, respiratory-risk users, and outdoor workers

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For open-data air-quality notification reuse case, resolve target users and pollution-season context.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish air-quality notification from air-quality regulation, target users from all residents, spring dust episodes from annual pollution averages, and reuse-case description from measured health impact. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 10. BND-CORE-PAIR-045

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: climate-related displacement evidence in sub-Saharan Africa
answer_unit: estimated net displacement from temperature and rainfall anomalies

source_anchor:
- Climate-adaptation review text says temperature and rainfall anomalies in sub-Saharan Africa were estimated to have caused net displacement of 5 million people during the studied period.

internal_source_boundary:
- source_name: internal climate-adaptation evidence source bundle
- source_scope: paragraph on adverse weather events, sub-Saharan Africa, temperature and rainfall anomalies, and net displacement estimate

final_prompt_text:
Use the primary analytical source as anchor and one corroborating source if available. For climate-related displacement evidence in sub-Saharan Africa, resolve estimated net displacement from temperature and rainfall anomalies.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish net displacement from gross migration flows, weather anomalies from long-run climate averages, regional estimate from country-specific effects, and cited study result from global displacement totals. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 11. BND-CORE-PAIR-041

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: gender-sensitive public-procurement mandate coverage
answer_unit: share of economies mandating gender-sensitive criteria and procurement-market scale

source_anchor:
- Legal/economic indicators text says less than one in five economies mandate gender-sensitive criteria for public procurement.
- It says women are largely cut out of a nearly USD 10 trillion a year procurement market.

internal_source_boundary:
- source_name: internal gender-and-law indicators source bundle
- source_scope: paragraph on gender-sensitive public procurement criteria and annual public-procurement market scale

final_prompt_text:
Use the official indicators source as anchor and one corroborating source if available. For gender-sensitive public-procurement mandate coverage, resolve share of economies mandating gender-sensitive criteria and procurement-market scale.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish mandated criteria from voluntary procurement practices, economies from countries in a region, market scale from spending accessible to women-owned firms, and annual global estimate from domestic procurement totals. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 12. BND-CORE-PAIR-021

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Australia clean-energy workforce training programmes
answer_unit: apprenticeship support target and related vocational-training initiative

source_anchor:
- Country labour note says the New Energy Apprenticeship Program seeks to support 10,000 apprentices in the clean and renewable energy sector.
- It says a fee-free vocational education initiative will deliver 180,000 courses for priority groups in in-demand occupations, including occupations key to the energy transition.

internal_source_boundary:
- source_name: internal employment-outlook country-note source bundle
- source_scope: Australia paragraph on clean-energy transition training, apprenticeship target, and fee-free vocational courses

final_prompt_text:
Use the official labour-market note as anchor and one corroborating source if available. For Australia clean-energy workforce training programmes, resolve apprenticeship support target and related vocational-training initiative.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish apprentices supported from courses delivered, clean-energy apprenticeships from all vocational training, priority groups from total workforce, and programme target from completed participation. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 13. CORE-SCI-03

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: education-ministry teacher-shortage policy focus
answer_unit: attraction versus retention emphasis

source_anchor:
- Education policy text says a larger share of education ministries are focused on attracting teachers compared with retaining them.
- It frames the issue as an urgent challenge of teacher shortages and matching teacher supply and demand.

internal_source_boundary:
- source_name: internal teaching-profession policy source bundle
- source_scope: paragraph on teacher shortages, supply-demand matching, attraction policies, and retention policies

final_prompt_text:
Use the official education policy source as anchor and one corroborating source if available. For education-ministry teacher-shortage policy focus, resolve attraction versus retention emphasis.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish ministry policy focus from measured teacher vacancies, attraction from retention, ageing-workforce concerns from technology-adoption support, and cross-system pattern from one country's staffing policy. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 14. CORE-POL-33

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: marine geospatial information public-benefit assessment
answer_unit: assessment year and conclusion about societal need

source_anchor:
- Country-response text says an assessment of the societal benefit of a marine geospatial information service was made in 2020.
- It says the report concluded that the service fulfils an important societal need.

internal_source_boundary:
- source_name: internal open-data reuse country-response source bundle
- source_scope: paragraph on marine geospatial information, 2020 societal-benefit assessment, and conclusion about societal need

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For marine geospatial information public-benefit assessment, resolve assessment year and conclusion about societal need.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish societal-benefit assessment from usage analytics, marine geospatial information from all geospatial data, assessment conclusion from quantified economic value, and 2020 assessment from later portal updates. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 15. CORE-POL-24

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: high-value-dataset implementation progress scale
answer_unit: progress-score scale and organisational/legal/technical dimensions

source_anchor:
- Questionnaire table text lists categories of high-value datasets and answers for 2024.
- It shows degree of progress from 1 to 5 across organisational, legal, and technical progress dimensions.

internal_source_boundary:
- source_name: internal open-data questionnaire source bundle
- source_scope: high-value-dataset table rows on 2024 progress scores and organisational, legal, and technical dimensions

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For high-value-dataset implementation progress scale, resolve progress-score scale and organisational/legal/technical dimensions.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish progress score from dataset count, organisational progress from legal and technical progress, high-value dataset categories from all open data, and 2024 self-reported answers from later compliance status. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 16. CORE-POL-10

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Bulgaria open-data governance support in 2024
answer_unit: national strategy basis and publishing-support institution

source_anchor:
- Country factsheet text says open-data principles are embedded in a national e-government strategy for 2019-2025.
- It says the ministry responsible for e-government supports administrations in dataset publishing.

internal_source_boundary:
- source_name: internal open-data maturity country-factsheet source bundle
- source_scope: Bulgaria factsheet paragraph on national e-government strategy, open-data principles, and institutional support for dataset publishing

final_prompt_text:
Use the official country factsheet as anchor and one corroborating source if available. For Bulgaria open-data governance support in 2024, resolve national strategy basis and publishing-support institution.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish national strategy basis from portal maturity score, publishing support from mandatory dataset contribution, e-government strategy from open-data-only strategy, and 2024 factsheet status from later legislative updates. Return: current classification with boundary note, source comparison, caveat, and confidence.
