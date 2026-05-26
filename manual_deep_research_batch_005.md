# Manual Deep-Research Prompt Batch 005

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

## 1. CORE-ECON-12

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: France short-term macroeconomic forecast
answer_unit: headline inflation projection for 2024 and 2025

source_anchor:
- Forecast text says headline inflation is expected to recede to 2.3% in 2024 and 2.0% in 2025.

internal_source_boundary:
- source_name: internal macroeconomic forecast source bundle
- source_scope: France forecast paragraph on inflation, purchasing power, public support programmes, and GDP growth

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For France short-term macroeconomic forecast, resolve headline inflation projection for 2024 and 2025.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish headline versus core inflation, forecast year versus publication year, annual average versus end-period rate, and revised versus earlier projections. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 2. CORE-ECON-14

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: India population-rank transition
answer_unit: year India surpassed China as the world's most populous country

source_anchor:
- Demographic text states that India surpassed China as the world's most populous country in 2023.

internal_source_boundary:
- source_name: internal demographic indicators source bundle
- source_scope: population-growth paragraph naming India, China, and projected contributors to global population increase

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For India population-rank transition, resolve the year India surpassed China as the world's most populous country.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish calendar-year crossover, mid-year population estimates, projection revisions, and "largest country" by population rather than land area or economy. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 3. BND-CORE-PAIR-017

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Germany labour-market status in May 2024
answer_unit: unemployment rate and comparison with pre-pandemic and crisis levels

source_anchor:
- Labour-market note reports Germany's unemployment rate as 3.3% in May 2024.
- The same passage compares it with 3.1% in December 2019 and a 3.9% crisis peak in late 2020 or early 2021.

internal_source_boundary:
- source_name: internal employment-outlook country-note source bundle
- source_scope: Germany labour-market paragraph covering May 2024 unemployment, December 2019 comparison, and late-2020 or early-2021 peak

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For Germany labour-market status in May 2024, resolve the unemployment rate and how it compares with pre-pandemic and crisis levels.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish seasonally adjusted unemployment from employment rate, national definitions from harmonised rates, point-in-time May data from quarterly values, and crisis peak timing. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 4. CORE-GEN-07

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: 2024 Gen Z and millennial financial-stress survey
answer_unit: global shares living paycheck-to-paycheck and change versus prior year

source_anchor:
- Survey summary says roughly six in ten Gen Zs and millennials live paycheck-to-paycheck.
- It gives 56% for Gen Zs and 55% for millennials, up five points for Gen Zs.

internal_source_boundary:
- source_name: internal workforce survey source bundle
- source_scope: 2024 survey summary lines on paycheck-to-paycheck shares for Gen Zs and millennials

final_prompt_text:
Use the underlying survey report as anchor and one corroborating source if available. For 2024 Gen Z and millennial financial-stress survey, resolve global shares living paycheck-to-paycheck and the reported change versus the prior year.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish global survey results from country-specific cuts, Gen Z versus millennial cohorts, percentage-point change versus relative change, and fieldwork year versus report year. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 5. CORE-POL-02

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: global carbon-pricing revenue in 2023
answer_unit: total revenue from carbon taxes and emissions trading systems

source_anchor:
- Source text says carbon pricing revenues exceeded USD 100 billion for the first time in 2023.
- It gives total revenues from carbon taxes and ETSs as USD 104 billion, around a 4% real increase.

internal_source_boundary:
- source_name: internal carbon-pricing report source bundle
- source_scope: paragraph on 2023 carbon-pricing revenues and government revenue share

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For global carbon-pricing revenue in 2023, resolve total revenue from carbon taxes and emissions trading systems.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish carbon taxes from emissions trading systems, nominal totals from real-change statements, global aggregate from country coverage, and revenue collected in 2023 from later publication updates. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 6. CORE-POL-05

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: acute public-health event reporting by region
answer_unit: regional concentration of reported events in recent years

source_anchor:
- Health-emergency text says events reported from the African Region and the Region of the Americas consistently make up approximately 50% of all events in recent years.
- A related figure covers countries, territories, and areas reporting at least one acute public health event by region for 2018-2022.

internal_source_boundary:
- source_name: internal global health emergency source bundle
- source_scope: paragraph and figure note on acute public health event reporting by region, 2018-2022

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For acute public-health event reporting by region, resolve the regional concentration of reported events in recent years.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish event counts from countries reporting at least one event, reporting regions from geographic incidence, "recent years" from the 2018-2022 figure window, and surveillance bias from actual disease burden. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 7. CORE-POL-45

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: AI-system dataset quality obligation
answer_unit: required qualities for training, validation, and testing data

source_anchor:
- Legal text says training, validation, and testing datasets, including labels, should be relevant, sufficiently representative, and to the best extent possible free of errors and complete in view of the system's intended purpose.

internal_source_boundary:
- source_name: internal AI regulation source bundle
- source_scope: legal paragraph on training, validation, and testing data quality for AI systems

final_prompt_text:
Use the controlling legal text as anchor and one corroborating source if available. For AI-system dataset quality obligation, resolve required qualities for training, validation, and testing data.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish binding legal requirements from recitals or guidance, training data from validation and testing data, labels from underlying data, and "to the best extent possible" from absolute guarantees. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 8. CORE-TECH-21

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: GovTech collaboration strategy adoption
answer_unit: shares using GovTech for innovation and technology testing

source_anchor:
- Digital-government text says 55% are using GovTech to foster innovation, experimentation, and collaboration.
- It also says 42% are using GovTech to facilitate testing and adoption of technologies.

internal_source_boundary:
- source_name: internal digital-government policy source bundle
- source_scope: GovTech strategy bullets on innovation, experimentation, collaboration, testing, and adoption

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For GovTech collaboration strategy adoption, resolve shares using GovTech for innovation and technology testing.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish survey respondents from all governments, strategy use from measured implementation, innovation-culture goals from technology-testing goals, and percentage shares from counts of countries. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 9. CORE-TECH-03

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: recreational screen-use survey
answer_unit: share reporting over five hours of daily recreational screen use and highest age group

source_anchor:
- Survey brief says about 38% of respondents report over five hours of daily recreational screen use.
- It identifies the 18-25 age group as highest at 41%.

internal_source_boundary:
- source_name: internal digital-engagement survey source bundle
- source_scope: survey bullets on recreational screen use, age groups, and adult screen-use guidance

final_prompt_text:
Use the underlying survey brief as anchor and one corroborating source if available. For recreational screen-use survey, resolve the share reporting over five hours of daily recreational screen use and the highest age group.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish recreational from work or school screen time, all respondents from age subgroups, self-reported survey shares from clinical guidance, and age-band labels across summaries. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 10. CORE-GEN-02

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: blue-economy results-framework update
answer_unit: decision timing and reason for updating the results framework

source_anchor:
- Programme progress text says the context evolved during 2021, 2022, and 2023.
- It says a decision to update the results framework was made during the Ninth Partnership Council meeting in Ghana in June 2023.

internal_source_boundary:
- source_name: internal programme progress source bundle
- source_scope: results-framework paragraph covering 2021-2023 monitoring context, Ninth Partnership Council decision, and updated M&E plan

final_prompt_text:
Use the official programme source as anchor and one corroborating source if available. For blue-economy results-framework update, resolve decision timing and reason for updating the results framework.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish a decision to update from final adoption, monitoring-year context from fiscal-year progress, donor meeting location from programme scope, and results framework from individual output indicators. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 11. CORE-POL-22

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Sweden open-data maturity assessment
answer_unit: 2024 dimension structure and reuse-measurement status

source_anchor:
- Country factsheet text says open-data maturity is measured across policy, portal, quality, and impact.
- It says each dimension contributes an equal 25% toward the overall maturity score and that Sweden has processes to monitor reuse.

internal_source_boundary:
- source_name: internal open-data maturity country-factsheet source bundle
- source_scope: Sweden factsheet paragraphs on methodology, four dimensions, impact, and reuse-monitoring questions

final_prompt_text:
Use the official country factsheet as anchor and one corroborating source if available. For Sweden open-data maturity assessment, resolve the 2024 dimension structure and reuse-measurement status.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish overall maturity score from dimension scores, equal weighting from country performance, reuse monitoring from impact measurement methodology, and country factsheet text from cross-country portal summaries. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 12. CORE-POL-13

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Finland open-data policy controls
answer_unit: action-plan status and metadata-quality monitoring status

source_anchor:
- Country factsheet text asks whether the national open-data policy or strategy includes an action plan and records "Yes".
- It also asks whether metadata quality available on the portal is monitored and records "No".

internal_source_boundary:
- source_name: internal open-data maturity country-factsheet source bundle
- source_scope: Finland factsheet key-question rows on action plan, policy implementation processes, metadata quality monitoring, and reuse monitoring

final_prompt_text:
Use the official country factsheet as anchor and one corroborating source if available. For Finland open-data policy controls, resolve action-plan status and metadata-quality monitoring status.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish action-plan existence from implementation processes, metadata-quality monitoring from dataset-quality scoring, country-specific answers from neighbouring country factsheets, and 2024 status from later portal updates. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 13. CORE-POL-15

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Ireland open-data policy controls
answer_unit: action-plan status and metadata-quality monitoring status

source_anchor:
- Country factsheet text says Ireland employs tracking, surveys, feedback, workshops, conferences, and collaboration for open-data work.
- It records "Yes" for action-plan status and "Yes" for monitoring metadata quality on the portal.

internal_source_boundary:
- source_name: internal open-data maturity country-factsheet source bundle
- source_scope: Ireland factsheet key-question rows on action plan, metadata quality monitoring, and user-feedback processes

final_prompt_text:
Use the official country factsheet as anchor and one corroborating source if available. For Ireland open-data policy controls, resolve action-plan status and metadata-quality monitoring status.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish the policy action plan from operational feedback tools, metadata-quality monitoring from user-satisfaction monitoring, country-specific factsheet answers from adjacent country records, and 2024 status from later national portal changes. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 14. BND-CORE-PAIR-006

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: global oil-demand outlook to 2030
answer_unit: projected level where demand levels off toward the end of the decade

source_anchor:
- Energy forecast text says global oil demand will level off at around 106 mb/d toward the end of the decade under today's market conditions and policies.

internal_source_boundary:
- source_name: internal oil-market forecast source bundle
- source_scope: executive-summary paragraph on clean energy transition and global oil-demand level toward 2030

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For global oil-demand outlook to 2030, resolve projected level where demand levels off toward the end of the decade.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish oil demand from supply capacity, mb/d from annual barrels, policy-stated forecast from net-zero scenarios, and "toward end of decade" from a single calendar-year observation. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 15. CORE-ECON-20

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Viet Nam 2024 growth forecast
answer_unit: real GDP growth projection and key assumption

source_anchor:
- Country outlook text says Viet Nam's economy is forecast to grow by 5.5% in 2024.
- It says this projection assumes a continued recovery of manufacturing exports.

internal_source_boundary:
- source_name: internal country economic update source bundle
- source_scope: Viet Nam outlook paragraph covering 2023 deceleration, 2024 growth forecast, assumptions, and risks

final_prompt_text:
Use the official country outlook as anchor and one corroborating source if available. For Viet Nam 2024 growth forecast, resolve real GDP growth projection and key assumption.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish real GDP from nominal or export growth, forecast year from publication year, baseline assumption from upside or downside risks, and latest update from earlier projections. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 16. CORE-SCI-04

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: TALIS 2024 coverage caution
answer_unit: countries and ISCED levels requiring caution in comparison with 2018

source_anchor:
- Survey documentation says caution is required when interpreting estimates for countries and territories that did not meet target population coverage in both TALIS 2018 and TALIS 2024.
- It lists ISCED level 1 teacher and principal data for Australia and the Netherlands, and ISCED level 2 principal data for Australia.

internal_source_boundary:
- source_name: internal education survey methodology source bundle
- source_scope: coverage-caution note comparing TALIS 2018 and TALIS 2024 by country, ISCED level, and respondent type

final_prompt_text:
Use the official survey methodology source as anchor and one corroborating source if available. For international teaching-survey coverage caution in 2024, resolve countries and ISCED levels requiring caution in comparison with 2018.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish teacher data from principal data, ISCED level 1 from ISCED level 2, coverage caution from low response-rate caution, and cross-cycle comparability from one-year estimates. Return: current classification with boundary note, source comparison, caveat, and confidence.
