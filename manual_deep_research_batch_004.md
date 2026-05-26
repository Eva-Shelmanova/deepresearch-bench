# Manual Deep-Research Prompt Batch 004

Runnable benchmark items only. This file uses a hybrid deep-research benchmark method: each prompt keeps one research object and one answer target, but requires source comparison, boundary/methodology judgement, discrepancy handling, and confidence rather than a single-fact lookup.

Mandatory rule:
- Core = one object + one disputed or methodology-sensitive parameter + one trap about definitions, dates, reporting scope, or update status.
- Set = one explicit `candidate_item` + one real boundary condition; the prompt must not merely ask whether the item appears in a list.
- Use the official primary source as the anchor, and at least one corroborating secondary source where available. If one primary register, legal act, or official table is controlling, explain why and use other sources only to check revisions, naming, boundary conflicts, or later summaries.
- Answer format: conclusion, source comparison, caveat, and confidence level.
- Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond that boundary.
- Include a trend or update signal only when the source context makes time change relevant.
- Do not ask for broad list retrieval or an essay unrelated to the named research object.

---

## 1. CORE-ECON-17

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Microsoft shareholder distributions
answer_unit: quarterly dividend per share amount in fiscal 2024

source_anchor:
- Fiscal-year 2024 dividend rows show a per-share amount of $0.75.

internal_source_boundary:
- source_name: internal company annual-report source bundle
- source_scope: dividend table rows for fiscal year 2024

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For Microsoft shareholder distributions, resolve quarterly dividend per share amount in fiscal 2024.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish declared, paid, and record-date dividends; quarterly versus annualized amount; and fiscal-year versus calendar-year reporting. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 2. CORE-ECON-06

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Citigroup share repurchase authorization
answer_unit: $20 billion multiyear common stock repurchase programme and $1.5 billion planned first-quarter repurchases

source_anchor:
- On 13 January 2025, the board authorized a new multiyear $20 billion common stock repurchase program, with planned repurchases of $1.5 billion during the first quarter of 2025.

internal_source_boundary:
- source_name: internal bank annual-report source bundle
- source_scope: paragraph about 2025 repurchase authorization and planned first-quarter repurchases

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For Citigroup share repurchase authorization, resolve $20 billion multiyear common stock repurchase programme and $1.5 billion planned first-quarter repurchases.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish board authorization, planned repurchases, executed buybacks, remaining authorization, and quarter-specific versus multiyear amounts. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 3. BND-CORE-PAIR-015

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: Nestle advertising and marketing spend
answer_unit: 8.1% of sales in 2024 and 9% target by end-2025

source_anchor:
- Advertising and marketing spend as a percentage of sales recovered to 8.1% in 2024 and is planned to increase further to 9% by the end of 2025.

internal_source_boundary:
- source_name: internal consumer-goods annual-review source bundle
- source_scope: sentence about advertising and marketing spend as percentage of sales

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For Nestle advertising and marketing spend, resolve 8.1% of sales in 2024 and 9% target by end-2025.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish actual 2024 spend from the end-2025 target, percentage of sales from absolute spend, and reported actuals from management plans. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 4. CORE-SCI-09

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: Ukraine reconstruction needs estimate
answer_unit: US$486 billion, equivalent to 2.8 times estimated 2023 nominal GDP

source_anchor:
- Reconstruction needs are estimated at US$486 billion, equivalent to 2.8 times the country's estimated 2023 nominal GDP.

internal_source_boundary:
- source_name: internal education/reconstruction source bundle
- source_scope: sentence about reconstruction needs and GDP multiple

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For Ukraine reconstruction needs estimate, resolve US$486 billion, equivalent to 2.8 times estimated 2023 nominal GDP.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish total needs from damages or financing gaps, estimate date, reconstruction period, nominal GDP baseline, and whether later assessments revise the figure. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 5. CORE-SCI-07

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Netherlands teacher salary change
answer_unit: 25% nominal statutory salary increase between 2015 and 2023

source_anchor:
- In the Netherlands, between 2015 and 2023, nominal statutory salaries increased by 25% for lower secondary teachers with 15 years of experience.

internal_source_boundary:
- source_name: internal education indicators source bundle
- source_scope: sentence about lower secondary teacher salaries from 2015 to 2023

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For Netherlands teacher salary change, resolve 25% nominal statutory salary increase between 2015 and 2023.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish nominal from real salary change, statutory from actual compensation, teacher profile, education level, and reference years. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 6. CORE-ECON-11

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: OECD unemployment rate in May 2024
answer_unit: 4.9% unemployment rate in May 2024

source_anchor:
- By May 2024, the OECD unemployment rate was 4.9%.

internal_source_boundary:
- source_name: internal employment outlook source bundle
- source_scope: sentence about unemployment rate in May 2024

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For OECD unemployment rate in May 2024, resolve 4.9% unemployment rate in May 2024.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish harmonised area-wide rate from national rates, seasonally adjusted from unadjusted data, reference month, and population coverage. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 7. CORE-POL-06

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: EU digital-services residual error rate control metric
answer_unit: target below 2% and estimated 2024 result of 0.5%

source_anchor:
- The residual error rate target is below 2%, and the estimated 2024 result is 0.5%.

internal_source_boundary:
- source_name: internal digital-services annual activity source bundle
- source_scope: metric row about residual error rate target and 2024 result

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For EU digital-services residual error rate control metric, resolve target below 2% and estimated 2024 result of 0.5%.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish target threshold from estimated result, gross from residual error, reporting year, and whether the metric covers payments, controls, or audit findings. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 8. BND-CORE-PAIR-043

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: EU administrative burden reduction objective
answer_unit: 25-35% administrative burden reduction objective

source_anchor:
- The objective is to cut administrative burden by at least 25-35%.

internal_source_boundary:
- source_name: internal regulatory-simplification source bundle
- source_scope: sentence about administrative burden reduction objective

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For EU administrative burden reduction objective, resolve 25-35% administrative burden reduction objective.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish political objective from adopted simplification measures, administrative burden from compliance cost, and the 25% versus 35% scope. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 9. BND-CORE-PAIR-040

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: EU artificial-intelligence regulation timing
answer_unit: entry into force on 1 August 2024 and full applicability on 2 August 2026

source_anchor:
- The regulation entered into force on 1 August 2024 and will be fully applicable on 2 August 2026, with exceptions.

internal_source_boundary:
- source_name: internal digital-regulation source bundle
- source_scope: sentence about entry-into-force and full-applicability dates

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For EU artificial-intelligence regulation timing, resolve entry into force on 1 August 2024 and full applicability on 2 August 2026.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish entry into force, staged applicability, exceptions, delegated rules, and obligations that apply on different dates. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 10. CORE-SCI-12

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: regional school water-service availability
answer_unit: close to 50% availability in Sub-Saharan Africa and at least 90% in other regions

source_anchor:
- In Sub-Saharan Africa, water-related services are available in close to 50% of schools; in all other regions, these services are available in at least 90% of schools.

internal_source_boundary:
- source_name: internal education indicator source bundle
- source_scope: paragraph about water-related services in schools by region

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For regional school water-service availability, resolve close to 50% availability in Sub-Saharan Africa and at least 90% in other regions.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish school level, service definition, region grouping, latest data year, and whether the figure is measured or modelled. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 11. CORE-POL-03

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: OECD international protection grants
answer_unit: 676,000 refugees granted international protection in 2023 and 160,000 resettled refugees

source_anchor:
- OECD countries granted international protection to 676,000 refugees in 2023, including 160,000 new resettled refugees.

internal_source_boundary:
- source_name: internal migration outlook source bundle
- source_scope: sentence about 2023 international protection and resettlement figures

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For OECD international protection grants, resolve 676,000 refugees granted international protection in 2023 and 160,000 resettled refugees.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish protection grants from applications, resettlement from other protection channels, country coverage, reporting year, and revised totals. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 12. CORE-SCI-06

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: young adults without upper-secondary attainment
answer_unit: 12% in the UK versus improvement from 17% to 14% across the comparison group

source_anchor:
- At 12%, the share of young adults in the UK without upper-secondary attainment stagnated between 2016 and 2023, while it improved from 17% to 14% on average across the comparison group.

internal_source_boundary:
- source_name: internal education equity source bundle
- source_scope: sentence about young adults without upper-secondary attainment

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For young adults without upper-secondary attainment, resolve 12% in the UK versus improvement from 17% to 14% across the comparison group.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish age cohort, attainment definition, country-specific classification, reference year, and comparison-group average. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 13. SET-TECH-E02

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: Fire OS operating-system inventory entry
candidate_item: Fire OS
answer_unit: vendor or company grouping under which the candidate appears

internal_source_boundary:
- source_name: internal operating systems list
- source_scope: Fire OS entry and its immediately preceding vendor/company grouping

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For Fire OS operating-system inventory entry, resolve vendor or company grouping under which the candidate appears for Fire OS.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish operating-system product from vendor/platform grouping, Android-derived family, current versus historical status, and row entry from heading. Return: current classification with boundary note, source comparison, caveat, and confidence. Do not retrieve the whole list.

---

## 14. SET-TECH-F05

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: React web-framework comparison row
candidate_item: React
answer_unit: implementation language recorded for the candidate

internal_source_boundary:
- source_name: internal web framework/library list
- source_scope: React row, implementation-language column

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For React web-framework comparison row, resolve implementation language for React.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish library versus framework classification, implementation language from authoring language, row field from surrounding comparison table, and version/date ambiguity. Return: current classification with boundary note, source comparison, caveat, and confidence. Do not retrieve the whole list.

---

## 15. BND-SET-SET007

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: Tokyo largest-city population row
candidate_item: Tokyo
answer_unit: UN 2025 population estimate recorded for the candidate

internal_source_boundary:
- source_name: internal city list
- source_scope: Tokyo row, UN 2025 population estimates column

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For Tokyo largest-city population row, resolve UN 2025 population estimate for Tokyo.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish city proper, urban area, and metropolitan area, plus estimate year and projection source. Return: best-supported estimate or range, source comparison, caveat, and confidence. Do not retrieve the whole list.

---

## 16. BND-SET-SET012

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: India English-speaking population row
candidate_item: India
answer_unit: total English-speaking population recorded for the candidate

internal_source_boundary:
- source_name: internal country list
- source_scope: India row, total English speakers column

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For India English-speaking population row, resolve total English-speaking population for India.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish total speakers from native speakers, additional-language speakers, age group, survey year, and estimates versus census-derived values. Return: best-supported estimate or range, source comparison, caveat, and confidence. Do not retrieve the whole list.
