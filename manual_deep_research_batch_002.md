# Manual Deep-Research Prompt Batch 002

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

## 1. CORE-POL-39

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: countries driving global population growth to 2050
answer_unit: group of countries contributing more than half of projected global population increase through 2050

source_anchor:
- A small group of countries including DRC, Egypt, Ethiopia, India, Nigeria, Pakistan, the Philippines, and Tanzania is expected to contribute more than half of global population increase through 2050.

internal_source_boundary:
- source_name: internal demographic source bundle
- source_scope: paragraph about countries contributing more than half of population growth through 2050

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For countries driving global population growth to 2050, resolve group of countries contributing more than half of projected global population increase through 2050.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish projection variant, country grouping, time horizon, fertility/migration assumptions, and later projection revisions. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 2. BND-CORE-PAIR-018

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: France inflation forecast
answer_unit: forecast inflation rates for 2024 and 2025

source_anchor:
- Headline inflation is expected to recede to 2.3% in 2024 and 2.0% in 2025.

internal_source_boundary:
- source_name: internal France macro outlook source bundle
- source_scope: sentence about 2024 and 2025 headline inflation forecast

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For France inflation forecast, resolve forecast inflation rates for 2024 and 2025.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish forecast vintage, headline versus core or harmonised inflation, annual average versus point estimate, and later actuals or revisions. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 3. CORE-POL-09

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Albania open-data legal implementation
answer_unit: entry-into-force date of the open-data law

source_anchor:
- Albania enacted Law No. 33/2022 on Open Data and Reuse of Public Sector Information, which came into force on 29 April 2023.

internal_source_boundary:
- source_name: internal Albania open-data legal source bundle
- source_scope: sentence about Law No. 33/2022 and entry into force

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For Albania open-data legal implementation, resolve entry-into-force date of the open-data law.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish enactment, publication, legal entry into force, implementation deadline, and practical availability of reusable data. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 4. CORE-POL-21

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Slovenia dynamic public-sector data reuse
answer_unit: immediate reuse rule for dynamic data after collection

source_anchor:
- The Slovenian changes include immediate reuse of dynamic data after collection.

internal_source_boundary:
- source_name: internal Slovenia open-data reform source bundle
- source_scope: sentence about dynamic data being reusable immediately after collection

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For Slovenia dynamic public-sector data reuse, resolve immediate reuse rule for dynamic data after collection.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish dynamic data from static datasets, immediate reuse from API/real-time availability, and legal permission from actual implementation. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 5. CORE-TECH-02

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: EU technical support instrument budget
answer_unit: EUR 864 million budget

source_anchor:
- Technical support has a budget of EUR 864 million for Member State structural reforms.

internal_source_boundary:
- source_name: internal digital policy / structural reform support source bundle
- source_scope: sentence about the EUR 864 million technical-support budget

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For EU technical support instrument budget, resolve EUR 864 million budget.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish programme envelope, annual commitments, payments, current-euro amounts, and the eligible reform scope. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 6. CORE-ECON-13

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: OECD unemployment rate in May 2024
answer_unit: unemployment rate around May 2024

source_anchor:
- By May 2024 the unemployment rate across the country group was 4.9%.

internal_source_boundary:
- source_name: internal labour-market outlook source bundle
- source_scope: sentence about unemployment rate in May 2024

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For OECD unemployment rate in May 2024, resolve unemployment rate around May 2024.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish harmonised area-wide rate from national rates, seasonally adjusted from unadjusted data, reference month, and population coverage. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 7. CORE-ECON-07

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: industrial company dividend and connected-machine target
answer_unit: EUR 1.15 dividend proposal and 80% by 2030 target distinction

source_anchor:
- The proposed 2024 dividend is EUR 1.15 per share, up 15 cents from the previous year.
- The company targets connecting 80% of enabled installed machines for digital applications by 2030.

internal_source_boundary:
- source_name: internal company performance source bundle
- source_scope: rows/sentences about dividend proposal and 2030 connected-machine target

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For industrial company dividend and connected-machine target, resolve EUR 1.15 dividend proposal and 80% by 2030 target distinction.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish proposed dividend from approved or paid dividend, and distinguish the connected-machine target denominator from installed-base or eligible-machine counts. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 8. CORE-POL-42

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_after_rewrite
research_object: public-sector data release exclusion rule
answer_unit: confidentiality, sensitivity, or lack-of-control limit on releasability

source_anchor:
- Some public-sector information cannot be released because it is confidential, sensitive, or not fully controlled by the administration.

internal_source_boundary:
- source_name: internal public-sector information reuse source bundle
- source_scope: sentence about confidentiality/sensitivity/control limits

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For public-sector data release exclusion rule, resolve confidentiality, sensitivity, or lack-of-control limit on releasability.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish legal exclusions for confidentiality, sensitivity, third-party rights, and lack of administrative control from general open-data policy statements. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 9. CORE-TECH-16

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: cybersecurity incident-reporting simplification
answer_unit: single cybersecurity incident-reporting mechanism

source_anchor:
- A digital simplification proposal includes a single mechanism for related cybersecurity incident reporting obligations.

internal_source_boundary:
- source_name: internal digital simplification source bundle
- source_scope: sentence about single cybersecurity incident-reporting mechanism

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For cybersecurity incident-reporting simplification, resolve single cybersecurity incident-reporting mechanism.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish a proposed single reporting mechanism from adopted obligations, and separate incident categories, affected entities, and reporting channels. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 10. CORE-POL-38

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: family migration and care-worker dependants
answer_unit: 373,000 family migrants in 2023 and March 2024 dependant rule change

source_anchor:
- Family migration reached 373,000 in 2023, a 60% increase from 2022.
- From March 2024 new care workers under that visa can no longer bring family members.

internal_source_boundary:
- source_name: internal migration policy source bundle
- source_scope: rows/sentences about family migration and care-worker dependant rule change

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For family migration and care-worker dependants, resolve 373,000 family migrants in 2023 and March 2024 dependant rule change.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish visa grants, applications, arrivals, dependants, route category, reporting year, and the effective date of the care-worker rule change. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 11. SET-GEN-F04

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: United States nominal GDP row
candidate_item: United States
answer_unit: leading nominal GDP estimate recorded for the candidate

internal_source_boundary:
- source_name: internal nominal GDP country/economy list
- source_scope: United States row, leading nominal GDP estimate column

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For United States nominal GDP row, resolve leading nominal GDP estimate for United States.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish nominal versus PPP measures, current versus constant prices, forecast versus observed data, and table year. Return: best-supported estimate or range, source comparison, caveat, and confidence. Do not retrieve the whole list.

---

## 12. BND-SET-SET005

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: Australia sovereign-state row
candidate_item: Australia - Commonwealth of Australia
answer_unit: sovereignty/status category recorded for the candidate

internal_source_boundary:
- source_name: internal sovereign-state list
- source_scope: Australia / Commonwealth of Australia row, membership/status category column

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For Australia - Commonwealth of Australia in relation to Australia sovereign-state row, resolve sovereignty/status category.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish short-form name from formal name, UN membership status from sovereignty description, row label from explanatory note, and federation/commonwealth terminology. Return: current legal/status conclusion, source comparison, caveat, and confidence. Do not retrieve the whole list.

---

## 13. BND-SET-SET008

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: Banjul International Airport code row
candidate_item: Banjul International Airport
answer_unit: IATA code recorded for the candidate

internal_source_boundary:
- source_name: internal airports by IATA code list
- source_scope: Banjul International Airport row, IATA code field

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For Banjul International Airport code row, resolve IATA code for Banjul International Airport.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish current airport name from former name, IATA code from ICAO code, airport serving area from city name, and registry entry from secondary airport lists. Return: concise conclusion, source comparison, caveat, and confidence. Do not retrieve the whole list.

---

## 14. SET-TECH-E03

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: SQL programming-language boundary entry
candidate_item: SQL
answer_unit: language category used to justify inclusion of the candidate

internal_source_boundary:
- source_name: internal programming language list
- source_scope: SQL entry and inclusion note about domain-specific languages

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For SQL programming-language boundary entry, resolve language category used to justify inclusion of the candidate for SQL.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish programming language, query language, domain-specific language, dialect family, and exclusion of markup-only systems. Return: current classification with boundary note, source comparison, caveat, and confidence. Do not retrieve the whole list.

---

## 15. SET-GEN-F05

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: Australia literacy-rate row
candidate_item: Australia
answer_unit: adult literacy-rate value recorded for the candidate

internal_source_boundary:
- source_name: internal literacy-rate country/economy list
- source_scope: Australia row, adult literacy-rate column

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For Australia literacy-rate row, resolve adult literacy-rate value for Australia.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish adult/youth literacy, estimate year, missing-value treatment, country/economy row naming, and primary data versus secondary compilation. Return: best-supported estimate or range, source comparison, caveat, and confidence. Do not retrieve the whole list.

---

## 16. SET-SCI-E01

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: CHEA accreditation-organisation entry
candidate_item: Council for Higher Education Accreditation
answer_unit: accreditation-organisation category recorded for the candidate

internal_source_boundary:
- source_name: internal educational accreditation organisation list
- source_scope: Council for Higher Education Accreditation entry and surrounding organisation-category context

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For Council for Higher Education Accreditation in relation to CHEA accreditation-organisation entry, resolve accreditation-organisation category.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish organisation name from accreditation category, institutional role from government recognition, regional heading from row entry, and primary registry from secondary compilation. Return: current legal/status conclusion, source comparison, caveat, and confidence. Do not retrieve the whole list.
