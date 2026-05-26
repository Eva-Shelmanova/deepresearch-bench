# Manual Deep-Research Prompt Batch 007

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

## 1. BND-CORE-PAIR-007

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: large online retailer 2024 revenue growth
answer_unit: total revenue growth rate and starting/ending revenue values

source_anchor:
- Annual-report text says total revenue grew 11% year over year.
- It gives the change as from $575B to $638B.

internal_source_boundary:
- source_name: internal company annual-report source bundle
- source_scope: revenue growth sentence giving total revenue, year-over-year rate, and beginning/ending revenue values

final_prompt_text:
Use the official company report as anchor and one corroborating source if available. For large online retailer 2024 revenue growth, resolve total revenue growth rate and starting/ending revenue values.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish total revenue from segment revenue, year-over-year growth from absolute dollar change, fiscal-year reporting from calendar-year headlines, and rounded billions from exact reported figures. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 2. BND-CORE-PAIR-023

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: balance-of-payments assistance programme status in 2024
answer_unit: whether new operations or repayments occurred and expected programme end

source_anchor:
- Financial-report text says no new operations or loan repayments occurred in 2024.
- It says the programme is expected to end in 2025 when the outstanding loan and related borrowing mature.

internal_source_boundary:
- source_name: internal institutional financial-report source bundle
- source_scope: paragraph on balance-of-payments assistance operations, repayments, outstanding loan, related borrowing, and expected end

final_prompt_text:
Use the official financial report as anchor and one corroborating source if available. For balance-of-payments assistance programme status in 2024, resolve whether new operations or repayments occurred and the expected programme end.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish new operations from loan repayments, programme end from loan maturity, 2024 activity from 2025 expected closure, and this assistance line from other lending facilities. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 3. BND-CORE-PAIR-053

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Green Line crossings in 2024
answer_unit: direction of change in Greek Cypriot crossings compared with the previous year

source_anchor:
- Implementation-report text says there was a decrease in 2024 compared with the previous year in the number of crossings by Greek Cypriots.

internal_source_boundary:
- source_name: internal border-implementation report source bundle
- source_scope: paragraph on authorised crossing points and 2024 change in crossings by Greek Cypriots

final_prompt_text:
Use the official implementation report as anchor and one corroborating source if available. For Green Line crossings in 2024, resolve the direction of change in Greek Cypriot crossings compared with the previous year.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish Greek Cypriot crossings from other EU or third-country crossings, authorised crossing points from total mobility, direction of change from absolute volume, and annual comparison from longer-term trend. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 4. CORE-POL-07

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: internal audit recommendation follow-up at January 2025 cut-off
answer_unit: accepted recommendations assessed as effectively implemented

source_anchor:
- Audit-report text says that as of 31 January 2025, 544 out of 831 partially accepted recommendations made in 2020-2024 were assessed by auditees as effectively implemented.
- It gives the share as 65%.

internal_source_boundary:
- source_name: internal annual internal-audit report source bundle
- source_scope: statistical paragraph on accepted recommendations, cut-off date, implementation status, numerator, denominator, and percentage

final_prompt_text:
Use the official audit report as anchor and one corroborating source if available. For internal audit recommendation follow-up at January 2025 cut-off, resolve accepted recommendations assessed as effectively implemented.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish accepted from all issued recommendations, auditee-assessed implementation from independently verified closure, partially accepted recommendations from fully accepted ones, and 2020-2024 recommendation population from 2024 audit work. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 5. CORE-POL-40

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: genetically engineered crop adaptation-ratio example
answer_unit: adaptation ratio implied by yield-loss offset and baseline heat effect

source_anchor:
- Climate-economics text says an additional hot day reduces yield by 0.293 units.
- It says genetically engineered varieties offset this yield loss by 0.0286 units, implying an adaptation ratio of 0.1.

internal_source_boundary:
- source_name: internal climate-adaptation evidence source bundle
- source_scope: paragraph explaining yield-loss coefficient, offset coefficient, and implied adaptation ratio

final_prompt_text:
Use the primary analytical source as anchor and one corroborating source if available. For genetically engineered crop adaptation-ratio example, resolve the adaptation ratio implied by yield-loss offset and baseline heat effect.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish coefficient ratio from percentage-point change, offset effect from full elimination of loss, crop-yield adaptation from general climate resilience, and study example from global average. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 6. CORE-GEN-09

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: China childlessness cohort-note definitions
answer_unit: birth cohorts and datasets used for reported China childlessness estimates

source_anchor:
- Social-indicator note says China's 1935 cohort refers to women born in 1931-1935 and the 1955 cohort to women born in 1951-1955.
- It says these data were calculated using the 1995 dataset, while the 1970 cohort used the 2015 dataset.

internal_source_boundary:
- source_name: internal social-indicator source bundle
- source_scope: figure note on permanent childlessness cohorts and China-specific cohort/dataset definitions

final_prompt_text:
Use the official statistical source as anchor and one corroborating source if available. For China childlessness cohort-note definitions, resolve birth cohorts and datasets used for reported childlessness estimates.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish cohort label from actual birth-year range, China-specific notes from general figure labels, permanent childlessness from fertility rate, and source dataset year from cohort year. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 7. BND-CORE-PAIR-010

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: cloud-accounting platform customer-acquisition cost
answer_unit: average cost per gross subscriber added and adjusted sales-marketing share

source_anchor:
- Annual-report text says the average cost of acquiring a subscriber increased to $598 per gross subscriber added.
- It says sales and marketing costs would have been 31.2% of operating revenue, 1.3 percentage points lower than the reported 32.5%.

internal_source_boundary:
- source_name: internal company annual-report source bundle
- source_scope: operating-cost paragraph on subscriber acquisition cost and adjusted sales-marketing share of operating revenue

final_prompt_text:
Use the official company report as anchor and one corroborating source if available. For cloud-accounting platform customer-acquisition cost, resolve average cost per gross subscriber added and adjusted sales-marketing share.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish gross subscriber added from net subscriber growth, average acquisition cost from total sales spend, adjusted percentage from reported percentage, and percentage-point difference from percent difference. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 8. BND-CORE-PAIR-012

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: AI automation labour-risk estimate
answer_unit: share of jobs in occupations at highest automation risk

source_anchor:
- Labour-market text says occupations at highest risk of automation account for about 28% of jobs.

internal_source_boundary:
- source_name: internal AI-and-labour-market source bundle
- source_scope: paragraph on AI effects on labour demand and occupation-level automation-risk estimate

final_prompt_text:
Use the official analytical source as anchor and one corroborating source if available. For AI automation labour-risk estimate, resolve share of jobs in occupations at highest automation risk.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish highest-risk occupations from all AI-exposed jobs, task substitution from job loss, occupation share from worker probability, and older task-based studies from later estimates that account for complementarity. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 9. BND-CORE-PAIR-020

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Japan gender employment gap context in 2024 labour note
answer_unit: gender employment gap and unpaid-care context

source_anchor:
- Labour-market note says Japan's gender employment gap is the fourth highest among peer countries at 21.3%.
- It says time spent on unpaid care and domestic work is also among the highest.

internal_source_boundary:
- source_name: internal employment-outlook country-note source bundle
- source_scope: Japan labour-market paragraph on gender employment gap and unpaid care/domestic work context

final_prompt_text:
Use the official labour-market note as anchor and one corroborating source if available. For Japan gender employment gap context in 2024 labour note, resolve the gender employment gap and unpaid-care context.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish employment gap from wage gap, ranking position from absolute value, unpaid-care time from paid employment, and cross-country benchmark group from domestic-only comparison. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 10. CORE-GEN-05

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: public-service satisfaction in trust survey
answer_unit: share of recent users satisfied with national health services

source_anchor:
- Trust-survey text says a majority of recent users of relevant public services report relative satisfaction with national health services.
- It gives the share as 52%.

internal_source_boundary:
- source_name: internal trust-survey source bundle
- source_scope: paragraph on public-service satisfaction and national health service share among recent users

final_prompt_text:
Use the official survey source as anchor and one corroborating source if available. For public-service satisfaction in trust survey, resolve the share of recent users satisfied with national health services.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish recent users from the whole population, national health services from all public services, relative satisfaction from trust in government, and survey wave from later releases. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 11. CORE-POL-18

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Netherlands open-data legal update and reuse monitoring
answer_unit: June 2024 legal implementation and portal reuse-monitoring methods

source_anchor:
- Country factsheet text says a public-sector information reuse act was adopted in June 2024 and fully implements a public-sector open-data directive.
- It says the national data portal analyses usage metrics and conducts user interviews, and that the statistical office hosts user days.

internal_source_boundary:
- source_name: internal open-data maturity country-factsheet source bundle
- source_scope: Netherlands factsheet paragraphs on June 2024 legal update, usage metrics, user interviews, and user days

final_prompt_text:
Use the official country factsheet as anchor and one corroborating source if available. For Netherlands open-data legal update and reuse monitoring, resolve the June 2024 legal implementation and portal reuse-monitoring methods.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish legal implementation from portal functionality, usage metrics from user interviews, user days from continuous analytics, and national factsheet status from neighbouring country records. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 12. CORE-POL-17

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Luxembourg parliamentary open-data reuse support
answer_unit: mechanisms used to support creative data reuse and media needs

source_anchor:
- Country factsheet text says the Parliament actively supports open data by publishing relevant datasets, incorporating journalist feedback, and organising hackathons.
- It says these actions are intended to drive creative data reuse and meet media needs.

internal_source_boundary:
- source_name: internal open-data maturity country-factsheet source bundle
- source_scope: Luxembourg factsheet paragraph on parliamentary dataset publication, journalist feedback, hackathons, and media needs

final_prompt_text:
Use the official country factsheet as anchor and one corroborating source if available. For Luxembourg parliamentary open-data reuse support, resolve mechanisms used to support creative data reuse and media needs.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish parliamentary open-data actions from national portal maturity scores, journalist feedback from general user feedback, hackathons from regular publication, and media needs from all reuse audiences. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 13. CORE-SCI-13

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Indonesia early-childhood centre principal survey
answer_unit: survey timing, population, and collection channel

source_anchor:
- Study text says data were collected in March 2022 through an electronic quantitative survey.
- It says the survey was made available via the education-data management platform to all registered early-childhood centres serving children from birth to age 6.

internal_source_boundary:
- source_name: internal early-childhood education study source bundle
- source_scope: methodology paragraph on survey timing, principal respondents, registered centres, age coverage, and electronic collection platform

final_prompt_text:
Use the primary study source as anchor and one corroborating source if available. For Indonesia early-childhood centre principal survey, resolve survey timing, population, and collection channel.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish registered centres from all centres, principals from teachers or parents, children birth-to-age-6 coverage from compulsory-school age, and electronic survey availability from completed response rate. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 14. CORE-TECH-01

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: African national cybersecurity institution coverage
answer_unit: number of surveyed countries with national CERTs and national cybersecurity strategies

source_anchor:
- Digital-governance text says that out of 44 African countries surveyed, 13 had a national CERT and 14 had a national cybersecurity strategy.
- It characterises the region as the weakest global performer on both indicators.

internal_source_boundary:
- source_name: internal digital-governance source bundle
- source_scope: paragraph on surveyed African countries, national CERT coverage, national cybersecurity strategies, and regional comparison

final_prompt_text:
Use the official digital-governance source as anchor and one corroborating source if available. For African national cybersecurity institution coverage, resolve the number of surveyed countries with national CERTs and national cybersecurity strategies.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish surveyed countries from all countries in the region, national CERT from broader incident-response capacity, cybersecurity strategy from cybersecurity law, and regional performance claim from individual-country status. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 15. BND-CORE-PAIR-025

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: private infrastructure investment market composition in 2023
answer_unit: primary-market growth and low- and middle-income country share in secondary markets

source_anchor:
- Infrastructure-finance text says private investment in infrastructure projects in primary markets increased by 10% in nominal terms in 2023.
- It says low- and middle-income countries represented around 12% of global secondary-market volumes.

internal_source_boundary:
- source_name: internal infrastructure investment report source bundle
- source_scope: paragraph on 2023 primary-market investment growth, developed-market contribution, LMIC secondary-market share, and 2024 preliminary rebound

final_prompt_text:
Use the official market report as anchor and one corroborating source if available. For private infrastructure investment market composition in 2023, resolve primary-market growth and low- and middle-income country share in secondary markets.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish primary markets from secondary markets, nominal growth from real growth, low- and middle-income country share from developed-market contribution, and 2023 observed data from preliminary 2024 rebound. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 16. BND-CORE-PAIR-028

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: regional open-data policy maturity dimension in 2024
answer_unit: average policy-dimension maturity level and change since 2023

source_anchor:
- Open-data maturity text says policy has been the most mature dimension on average since 2015.
- It reports the 2024 average as 91%, with a 2 percentage-point increase since 2023.

internal_source_boundary:
- source_name: internal open-data maturity report source bundle
- source_scope: maturity-report paragraph on 2024 policy dimension average, change since 2023, and comparison with other dimensions

final_prompt_text:
Use the official maturity report as anchor and one corroborating source if available. For regional open-data policy maturity dimension in 2024, resolve average policy-dimension maturity level and change since 2023.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish policy dimension from overall maturity score, percentage-point change from percent change, average regional maturity from individual-country results, and long-running dimension rank from a single-year score. Return: best-supported estimate or range, source comparison, caveat, and confidence.
