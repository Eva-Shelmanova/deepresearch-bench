# Manual Deep-Research Prompt Batch 006

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

## 1. BND-CORE-PAIR-054

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Netherlands regional working-age employment rates in 2023
answer_unit: national rate, regional range, and lowest/highest regions

source_anchor:
- Regional labour text defines the employment rate as employed persons out of the working-age population aged 15-64.
- It reports a national rate of 82.3%, a regional low of 79.1% in Limburg, and a high of 84.1% in North Brabant.

internal_source_boundary:
- source_name: internal regional employment source bundle
- source_scope: Netherlands 2023 employment-rate paragraph and regional values for working-age population aged 15-64

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For Netherlands regional working-age employment rates in 2023, resolve the national rate, regional range, and lowest/highest regions.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish employment rate from unemployment or participation rate, working-age population from total population, regional values from the national rate, and percentage points from percent change. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 2. BND-CORE-PAIR-019

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Korea labour-market status in May 2024
answer_unit: employment rate and comparison with May 2023 and December 2019

source_anchor:
- Country labour note reports Korea's employment rate for people aged 15-64 as 69.4% in May 2024.
- It says this was the same as May of the previous year and 2.2 percentage points above December 2019.

internal_source_boundary:
- source_name: internal employment-outlook country-note source bundle
- source_scope: Korea labour-market paragraph covering May 2024 employment rate and comparisons with May 2023 and December 2019

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For Korea labour-market status in May 2024, resolve the employment rate and comparison with May 2023 and December 2019.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish employment rate from unemployment rate, people aged 15-64 from all adults, seasonally adjusted values from raw values, and unchanged level from percentage-point increase versus pre-pandemic baseline. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 3. CORE-POL-04

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: occupation-shortage evidence for health and social care
answer_unit: period and evidence basis used to identify shortages

source_anchor:
- Workforce text says information on occupations in shortage covers the period spanning 2022 and 2023.
- It notes that the information draws on diverse sources and indicators, including public employment services' administrative data.

internal_source_boundary:
- source_name: internal health-workforce policy source bundle
- source_scope: paragraph on occupations in shortage, health and social care sector, reference period, and evidence sources

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For occupation-shortage evidence for health and social care, resolve the period and evidence basis used to identify shortages.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish shortage evidence from employment totals, health and social care from all sectors, administrative indicators from survey perceptions, and 2022-2023 evidence from later policy responses. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 4. CORE-SCI-02

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: education-attainment gender gap among young adults
answer_unit: young women and young men tertiary-qualification shares

source_anchor:
- Education text says women are more likely to pursue tertiary education.
- It reports 54% of young women holding a tertiary qualification compared with 41% of young men.

internal_source_boundary:
- source_name: internal education indicators source bundle
- source_scope: equity-themed education paragraph on tertiary qualification shares by gender among young adults

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For education-attainment gender gap among young adults, resolve young women and young men tertiary-qualification shares.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish young-adult attainment from all-adult attainment, tertiary qualification from upper-secondary completion, percentage-point gender gap from relative ratio, and cross-country aggregate from a single-country figure. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 5. CORE-SCI-16

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: child overweight and obesity regional distribution in 2024
answer_unit: Africa increase since 2000 and Asia share of under-5 cases

source_anchor:
- Health text says the number of overweight children under 5 in Africa has increased by nearly 12.1% since 2000.
- It says almost half of children under 5 who were overweight or living with obesity in 2024 lived in Asia.

internal_source_boundary:
- source_name: internal child-health indicators source bundle
- source_scope: obesity paragraph covering under-5 regional change since 2000 and regional distribution in 2024

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For child overweight and obesity regional distribution in 2024, resolve Africa's increase since 2000 and Asia's share of under-5 cases.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish overweight from obesity-only measures, children under 5 from children and adolescents, regional counts from prevalence rates, and 2024 estimates from long-run change since 2000. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 6. BND-CORE-PAIR-046

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: macroeconomic imbalance scoreboard export-performance indicator
answer_unit: 2024 status change and threshold

source_anchor:
- Scoreboard-review text says export performance against advanced economies is upgraded from auxiliary to headline indicator.
- It says the indicator is measured as the change over three years and has a newly established threshold of -3%.

internal_source_boundary:
- source_name: internal macroeconomic imbalance scoreboard source bundle
- source_scope: 2024 scoreboard review paragraph on export-performance indicator status, measurement period, and threshold

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For macroeconomic imbalance scoreboard export-performance indicator, resolve the 2024 status change and threshold.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish headline from auxiliary indicators, export performance against advanced economies from export market share, three-year change from annual level, and threshold breach from automatic policy conclusion. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 7. BND-CORE-PAIR-042

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: digital-service progression maturity metric
answer_unit: baseline, latest result, and maturity level

source_anchor:
- Internal reporting text gives a baseline of 24% in 2020 for the progression maturity metric.
- It reports the latest known result as 40%, Level 2 - Reactive, with a target to increase by the end of 2024.

internal_source_boundary:
- source_name: internal digital-services annual reporting source bundle
- source_scope: metric row on progression maturity level, 2020 baseline, end-2024 target, and latest known result

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For digital-service progression maturity metric, resolve the baseline, latest result, and maturity level.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish percentage metric from maturity-level label, baseline from target and latest result, end-2024 target wording from achieved status, and internal progression maturity from broader digital-government maturity. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 8. BND-CORE-PAIR-035

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: cohesion-policy performance-data reliability in 2024
answer_unit: whether reliability deficiencies led to suspension of interim payments

source_anchor:
- Internal control text says deficiencies in performance-data reliability are closely followed up and can lead to suspension of interim payments.
- It states that no such procedure was launched in 2024.

internal_source_boundary:
- source_name: internal cohesion-policy annual reporting source bundle
- source_scope: internal-control paragraph on reliability of performance data, audit follow-up, and suspension of interim payments in 2024

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For cohesion-policy performance-data reliability in 2024, resolve whether reliability deficiencies led to suspension of interim payments.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish potential suspension authority from an actual launched procedure, performance-data reliability from financial error rate, 2024 procedure status from later audit outcomes, and interim payments from programme selection rate. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 9. BND-CORE-PAIR-001

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: industrial-equipment company 2024 proposed dividend
answer_unit: proposed dividend per share and increase versus previous year

source_anchor:
- Annual-report text says the executive and supervisory boards will propose a payout of EUR 1.15 per share.
- It says this is an increase of 15 cents over the previous year.

internal_source_boundary:
- source_name: internal annual-report source bundle
- source_scope: dividend proposal paragraph for financial year 2024 and comparison with previous year

final_prompt_text:
Use the official company report as anchor and one corroborating source if available. For industrial-equipment company 2024 proposed dividend, resolve proposed dividend per share and increase versus previous year.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish proposed dividend from paid dividend, per-share amount from total payout, euro cents increase from percentage increase, and financial-year proposal from later shareholder approval. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 10. CORE-POL-36

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Spain open-data reuse-frequency survey
answer_unit: 2023 low-use share and missing-response caveat

source_anchor:
- Country response text says that in 2023, 29% use open data sometimes or almost never.
- It notes that 58% of respondents did not answer this question.

internal_source_boundary:
- source_name: internal open-data maturity country-response source bundle
- source_scope: Spain response paragraph on open-data reuse frequency in 2023 and non-response share

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For Spain open-data reuse-frequency survey, resolve the 2023 low-use share and missing-response caveat.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish "sometimes or almost never" from frequent use, respondent share from population share, non-response from zero use, and 2023 survey result from 2021 or 2019 comparisons. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 11. BND-CORE-PAIR-032

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: open-data impact survey methodology
answer_unit: 2023 survey basis and impact dimensions covered

source_anchor:
- Country response text says a 2023 survey on open-data impact was conducted.
- It says the survey is based on a national methodology inspired by European work and covers outputs, outcomes, and impacts across four dimensions.

internal_source_boundary:
- source_name: internal open-data maturity country-response source bundle
- source_scope: country response paragraph on 2023 open-data impact survey, methodology basis, and impact dimensions

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For open-data impact survey methodology, resolve the 2023 survey basis and impact dimensions covered.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish survey methodology from measured impact results, outputs from outcomes and impacts, national method from cross-country framework, and 2023 survey work from earlier impact studies. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 12. CORE-POL-26

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: open-data-supported pharmaceutical investigation
answer_unit: estimated value and role of official drug-control data

source_anchor:
- Country response text says an investigation uncovered illegal pharmaceutical activity worth EUR 20 million.
- It says the investigation was conducted by analysing open data from the state drug-control body and that many drugs ended up in pharmacies abroad.

internal_source_boundary:
- source_name: internal open-data reuse country-response source bundle
- source_scope: country response paragraph on pharmaceutical investigation, estimated value, and open-data source used

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For open-data-supported pharmaceutical investigation, resolve estimated value and role of official drug-control data.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish estimated value from recovered value, official drug-control open data from investigative conclusions, domestic pharmacy flow from foreign destinations, and reuse case description from legal case outcome. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 13. CORE-POL-35

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: open-data portal API analytics tooling
answer_unit: tool change from 2024 and API-usage monitoring status

source_anchor:
- Country response text records that API usage analytics are run.
- It says Google Analytics was used until 2024, then Matomo.

internal_source_boundary:
- source_name: internal open-data portal analytics source bundle
- source_scope: country response row on API usage analytics tools and change in 2024

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For open-data portal API analytics tooling, resolve tool change from 2024 and API-usage monitoring status.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish API analytics from general website analytics, tool migration from parallel tool use, "until 2024" from full-year 2024 coverage, and monitoring status from public reporting of metrics. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 14. CORE-TECH-06

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: AI risk measurement and monitoring practice
answer_unit: tracking mechanism requirement under the risk-measurement function

source_anchor:
- AI risk-management text says mechanisms for tracking identified AI risks over time are in place under a risk-measurement function.
- It links operations tasks to ongoing monitoring, periodic updates, testing, expert recalibration, and incident or error tracking.

internal_source_boundary:
- source_name: internal AI risk-management framework source bundle
- source_scope: risk-measurement function paragraph on tracking identified AI risks over time and operational monitoring tasks

final_prompt_text:
Use the controlling framework source as anchor and one corroborating source if available. For AI risk measurement and monitoring practice, resolve the tracking mechanism requirement under the risk-measurement function.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish risk measurement from risk mapping or management, tracking identified risks over time from one-time testing, operational monitoring from pre-deployment validation, and framework outcomes from legal obligations. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 15. CORE-TECH-12

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: federated learning privacy-preserving training model
answer_unit: core mechanism for collaborative training without raw-data transfer

source_anchor:
- Survey text says federated learning enables collaborative training of machine-learning models without needing to send raw, potentially sensitive data.
- It frames federated learning as a privacy-preserving technology for settings where data access is challenging.

internal_source_boundary:
- source_name: internal federated-learning survey source bundle
- source_scope: introduction paragraph defining federated learning and its privacy-preserving collaborative-training mechanism

final_prompt_text:
Use the primary survey source as anchor and one corroborating source if available. For federated learning privacy-preserving training model, resolve the core mechanism for collaborative training without raw-data transfer.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish federated learning from centralized data pooling, privacy preservation from formal privacy guarantees, model update exchange from raw-data transfer, and general definition from a specific deployment architecture. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 16. CORE-TECH-15

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: low-bit large-language-model quantization tradeoff
answer_unit: efficiency benefit and information-loss risk

source_anchor:
- Technical survey text says low-bit quantization can bring significant acceleration and parameter compression in inference.
- It also notes that it can lose information.

internal_source_boundary:
- source_name: internal low-bit language-model survey source bundle
- source_scope: survey paragraph on low-bit model quantization, acceleration, parameter compression, and information loss

final_prompt_text:
Use the primary survey source as anchor and one corroborating source if available. For low-bit large-language-model quantization tradeoff, resolve efficiency benefit and information-loss risk.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish parameter compression from runtime speedup, inference quantization from training-time quantization, information loss from measured accuracy degradation, and general low-bit methods from one named algorithm or hardware implementation. Return: concise conclusion, source comparison, caveat, and confidence.
