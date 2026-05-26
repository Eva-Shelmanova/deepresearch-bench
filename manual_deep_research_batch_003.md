# Manual Deep-Research Prompt Batch 003

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

## 1. CORE-POL-41

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: EU MIP scoreboard methodology
answer_unit: the -3% threshold for export performance against advanced economies

source_anchor:
- The 2024 MIP scoreboard review upgraded export performance against advanced economies and set a -3% threshold.

authoritative_sources:
- European Commission MIP scoreboard/report, EUR-Lex if needed

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For EU MIP scoreboard methodology, resolve the -3% threshold for export performance against advanced economies.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish the scoreboard threshold from a country result, an alert level, or a general export-growth target, and check whether the 2024 review changed the indicator definition or comparator group. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 2. CORE-SCI-11

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: Horizon Europe lump-sum funding simplification
answer_unit: the 50% lump-sum funding target by 2027

source_anchor:
- Horizon Europe simplification material refers to a target of lump-sum funding reaching 50% of call budgets by 2027.

authoritative_sources:
- European Commission Horizon Europe work programme, Horizon Europe implementation reports

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For Horizon Europe lump-sum funding simplification, resolve the 50% lump-sum funding target by 2027.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish a policy target from actual lump-sum uptake, call-budget coverage from project-count coverage, and a 2027 objective from interim implementation figures. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 3. CORE-TECH-17

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: DORA ICT incident monitoring
answer_unit: obligation to collect, monitor, and analyse ICT-related incidents or network performance issues

source_anchor:
- DORA delegated material says financial entities must collect, monitor, and analyse ICT network performance issues and ICT-related incidents.

authoritative_sources:
- EUR-Lex, European Commission, European Supervisory Authorities

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For DORA ICT incident monitoring, resolve obligation to collect, monitor, and analyse ICT-related incidents or network performance issues.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish adopted legal text, delegated/technical standards, incident monitoring, network-performance issues, and reporting obligations for different financial entities. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 4. CORE-POL-01

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: Poland Fiscal Council
answer_unit: planned start date of 1 January 2026

source_anchor:
- Poland's Fiscal Council is described as set to begin operations on 1 January 2026.

authoritative_sources:
- European Commission fiscal-governance material, Polish official legal/public finance sources

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For Poland Fiscal Council, resolve planned start date of 1 January 2026.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish legal establishment, appointment/setup milestones, budget-year applicability, and the date when the council is expected to begin operations. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 5. CORE-ECON-10

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: euro-area 2024 quarterly growth
answer_unit: Paris 2024 as a temporary Q3 growth factor

source_anchor:
- Euro-area growth accelerated in Q3 2024 partly because of temporary factors such as the Paris 2024 Olympic and Paralympic Games.

authoritative_sources:
- ECB 2024 euro-area economic reporting

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For euro-area 2024 quarterly growth, resolve Paris 2024 as a temporary Q3 growth factor.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish real GDP growth from temporary event effects, first estimates from later revisions, and one-off statistical boosts from underlying economic momentum. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 6. CORE-POL-12

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: open-data maturity dimension weights
answer_unit: four equally weighted maturity dimensions

source_anchor:
- Open data maturity is measured through policy, portal, quality, and impact, each contributing 25%.

authoritative_sources:
- data.europa.eu Open Data Maturity methodology/report

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For open-data maturity dimension weights, resolve four equally weighted maturity dimensions.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish methodology weights from country scores, dimension definitions, report year, and later methodology revisions. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 7. CORE-TECH-04

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: cryptocurrency electricity demand forecast
answer_unit: around 160 TWh by 2026

source_anchor:
- IEA electricity material projected cryptocurrency electricity consumption of around 160 TWh by 2026.

authoritative_sources:
- IEA Electricity report, recognised electricity-consumption trackers if needed

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For cryptocurrency electricity demand forecast, resolve around 160 TWh by 2026.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish proof-of-work mining from total cryptocurrency activity, network boundary, geography coverage, time window, and forecast methodology. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 8. CORE-TECH-19

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: Wuling Hongguang Mini EV affordability example
answer_unit: price around CNY 40,000

source_anchor:
- The Wuling Hongguang Mini EV is cited as priced around CNY 40,000.

authoritative_sources:
- IEA Global EV Outlook, manufacturer or market data if needed

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For Wuling Hongguang Mini EV affordability example, resolve price around CNY 40,000.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish model/version, listed price versus transaction price, subsidies or taxes, currency/date, and whether the source describes a launch price or current market price. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 9. CORE-POL-29

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: Hungary open meteorological data reuse
answer_unit: 5-7% balancing-energy cost reduction

source_anchor:
- Forecasting based on open-access meteorological data reportedly helped generators reduce balancing-energy costs by 5-7%.

authoritative_sources:
- data.europa.eu Open Data Maturity 2024 country evidence for Hungary

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For Hungary open meteorological data reuse, resolve 5-7% balancing-energy cost reduction.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish reported case-study savings from measured market-wide effects, cost-reduction denominator, forecasting method, and whether open data rather than other factors caused the result. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 10. SET-GEN-E01

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: Aachen Cathedral heritage-site entry
candidate_item: Aachen Cathedral
answer_unit: inscription year and criteria category recorded for the candidate
source_name: UNESCO World Heritage Centre
source_scope: Aachen Cathedral row, year-listed and criteria/type fields

authoritative_sources:
- UNESCO World Heritage Centre

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For Aachen Cathedral heritage-site entry, resolve inscription year and criteria category for Aachen Cathedral.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish inscription year, later boundary modifications, cultural/natural criteria, row entry, and name variants. Return: concise conclusion, source comparison, caveat, and confidence. Do not retrieve the whole list.

---

## 11. SET-GEN-E02

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: India population row
candidate_item: India
answer_unit: population value and world-population share recorded for the candidate
source_name: UN DESA World Population Prospects
source_scope: India row, population and percentage-of-world columns

authoritative_sources:
- UN DESA World Population Prospects

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For India population row, resolve population value and world-population share for India.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish country/area row, estimate date, latest revision, official estimate versus projection, and whether notes or dependencies change entity boundary. Return: best-supported estimate or range, source comparison, caveat, and confidence. Do not retrieve the whole list.

---

## 12. SET-GEN-E03

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: China GDP PPP row
candidate_item: China
answer_unit: leading GDP PPP estimate recorded for the candidate
source_name: World Bank World Development Indicators
source_scope: China row, leading GDP PPP estimate column

authoritative_sources:
- World Bank World Development Indicators

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For China GDP PPP row, resolve leading GDP PPP estimate for China.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish PPP from nominal GDP, current international dollars from other units, forecast year from observed year, and note-marked entity naming from entity identity. Return: best-supported estimate or range, source comparison, caveat, and confidence. Do not retrieve the whole list.

---

## 13. SET-GEN-F06

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: Canberra capital-city row
candidate_item: Canberra
answer_unit: country and continent recorded for the candidate
source_name: CIA World Factbook
source_scope: Canberra row, country/territory and continent fields

authoritative_sources:
- CIA World Factbook

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For Canberra capital-city row, resolve country and continent for Canberra.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish capital city from seat of government, country from territory/dependency scope, continent classification, and historical or de facto capital notes. Return: concise conclusion, source comparison, caveat, and confidence. Do not retrieve the whole list.

---

## 14. SET-TECH-F04

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: Mozilla Firefox browser-engine entry
candidate_item: Mozilla Firefox
answer_unit: browser-engine family recorded near the candidate
source_name: Wikipedia: List of web browsers
source_scope: Mozilla Firefox entry and surrounding browser-engine grouping

authoritative_sources:
- Wikipedia: List of web browsers

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For Mozilla Firefox browser-engine entry, resolve browser-engine family recorded near the candidate for Mozilla Firefox.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish browser product from browser engine, current browser from historical variants, engine family from vendor, and row entry from section heading. Return: current classification with boundary note, source comparison, caveat, and confidence. Do not retrieve the whole list.

---

## 15. BND-SET-SET020

task_type: online_multi_source_candidate_boundary_research
manual_status: ready
research_object: .png file-format entry
candidate_item: .png
answer_unit: file-format naming rule associated with the candidate
source_name: Wikipedia: List of file formats
source_scope: .png entry and lead note about lowercase file endings and format identifiers

authoritative_sources:
- Wikipedia: List of file formats

final_prompt_text:
Use the primary register/table as anchor and one corroborating source if available. For .png file-format entry, resolve file-format naming rule for .png.

Use `source_scope` only to locate the relevant row, note, heading, or paragraph; do not infer beyond it. Boundary trap: distinguish filename extension, file format, MIME/media type, file family, and whether the entry appears as a row, note, or example. Return: current classification with boundary note, source comparison, caveat, and confidence. Do not retrieve the whole list.
