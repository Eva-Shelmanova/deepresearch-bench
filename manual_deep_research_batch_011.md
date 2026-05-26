# Manual Deep-Research Prompt Batch 011

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

## 1. CORE-GEN-03

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: private infrastructure investment rebound in 2023-2024
answer_unit: primary-market growth rate and secondary-market share/rebound signal

source_anchor:
- Infrastructure-market text says private investment in infrastructure projects in primary markets rose by 10 percent in nominal terms in 2023.
- It says the low- and middle-income country share of secondary market volumes continued to decrease to around 12 percent, while preliminary 2024 data showed a rebound in secondary activity.

internal_source_boundary:
- source_name: internal infrastructure-market report source bundle
- source_scope: executive-summary paragraphs on 2023 primary-market investment growth, secondary-market share, and preliminary 2024 rebound signal

final_prompt_text:
Use the official infrastructure-market report as anchor and one corroborating source if available. For private infrastructure investment rebound in 2023-2024, resolve primary-market growth rate and secondary-market share/rebound signal.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish primary-market investment from secondary-market transactions, nominal growth from real growth, low- and middle-income-country share from global volume, and preliminary 2024 signal from final annual data. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 2. CORE-ECON-05

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: global oil-demand plateau outlook to 2030
answer_unit: projected demand level and transport-fuel savings components

source_anchor:
- Oil-market forecast text says global oil demand will level off at around 106 mb/d toward the end of the decade.
- It says electric-vehicle-related oil savings versus 2023 include 4.7 mb/d in gasoline and 1.4 mb/d in diesel, with commercial and freight use accounting for around 1 mb/d of diesel savings.

internal_source_boundary:
- source_name: internal oil-market forecast source bundle
- source_scope: executive-summary paragraphs on demand plateau, end-of-decade level, gasoline savings, diesel savings, and commercial/freight component

final_prompt_text:
Use the official energy-market forecast as anchor and one corroborating source if available. For global oil-demand plateau outlook to 2030, resolve projected demand level and transport-fuel savings components.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish demand level from annual growth, policy-based forecast from net-zero scenario, gasoline savings from diesel savings, and end-of-decade plateau from a precise 2030 point estimate. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 3. BND-CORE-PAIR-013

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: 2023 GDP growth versus GDP-per-capita divergence
answer_unit: countries with positive real GDP growth but falling real GDP per capita

source_anchor:
- Economic outlook text says Canada, Colombia, the Netherlands, New Zealand, Poland, and the United Kingdom all had positive real GDP growth in 2023 but a decline in real GDP per capita.
- The same source discusses broad trade rebound and financial-conditions context around 2023.

internal_source_boundary:
- source_name: internal economic-outlook source bundle
- source_scope: note identifying countries with positive real GDP growth in 2023 and declining real GDP per capita

final_prompt_text:
Use the official economic outlook as anchor and one corroborating source if available. For 2023 GDP growth versus GDP-per-capita divergence, resolve countries with positive real GDP growth but falling real GDP per capita.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish aggregate real GDP growth from real GDP per capita, calendar-year 2023 from forecast years, named country list from regional examples, and GDP-volume change from nominal income or exchange-rate effects. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 4. CORE-ECON-23

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: transportation-sector greenhouse-gas share in 2022
answer_unit: transport share of national emissions and comparative regional adoption shares

source_anchor:
- Macro-climate policy text says the transportation sector generated 36 percent of greenhouse gas emissions in the United States in 2022.
- It contrasts transport decarbonisation with other sectors and notes adoption shares for electric vehicles in major regions.

internal_source_boundary:
- source_name: internal climate-policy source bundle
- source_scope: paragraph on 2022 transport-sector greenhouse-gas share, emissions trend, and comparative regional electric-vehicle adoption shares

final_prompt_text:
Use the official analytical source as anchor and one corroborating source if available. For transportation-sector greenhouse-gas share in 2022, resolve transport share of national emissions and comparative regional adoption shares.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish transport-sector emissions from economy-wide emissions, national share from global or regional shares, greenhouse gases from carbon dioxide only, and adoption share from fleet stock or sales share. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 5. BND-CORE-PAIR-011

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: pandemic impact on global life expectancy
answer_unit: life-expectancy decline and excess-death framing

source_anchor:
- Global poverty-and-resilience text says the pandemic caused a significant number of excess deaths and reduced global life expectancy at birth by over 1.5 years.
- It discusses vulnerability, environmental risks, and resilience in lower-income settings.

internal_source_boundary:
- source_name: internal poverty-and-resilience report source bundle
- source_scope: overview paragraph on pandemic excess deaths and global life-expectancy decline

final_prompt_text:
Use the official global-development report as anchor and one corroborating source if available. For pandemic impact on global life expectancy, resolve life-expectancy decline and excess-death framing.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish period life expectancy at birth from cohort lifespan, excess deaths from confirmed deaths, global estimate from country-level mortality shocks, and pandemic effect from longer-run health trends. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 6. CORE-GEN-08

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: anti-corruption strategy implementation gap
answer_unit: share of planned strategy activities implemented and scope of strategic approach

source_anchor:
- Public-integrity outlook text says the majority of covered countries have a strategic approach to corruption.
- It says about two-thirds of planned activities in countries' strategies are implemented in practice.

internal_source_boundary:
- source_name: internal public-integrity outlook source bundle
- source_scope: introduction/executive-summary paragraphs on strategic anti-corruption approaches and implementation of planned activities

final_prompt_text:
Use the official public-integrity report as anchor and one corroborating source if available. For anti-corruption strategy implementation gap, resolve share of planned strategy activities implemented and scope of strategic approach.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish having a strategic approach from completing strategy actions, planned activities from outcomes, traditional corruption risks from newer integrity risks, and covered-country pattern from universal global coverage. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 7. CORE-ECON-18

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: dual-listed technology company regulatory-risk disclosure
answer_unit: concurrent listing requirements and AI-law risk context

source_anchor:
- Annual-report risk text says the company is subject to Hong Kong and United States listing and regulatory requirements concurrently.
- It says existing legal regimes regulate aspects of AI technologies and new laws regulating this area are being enacted.

internal_source_boundary:
- source_name: internal technology-company annual-report source bundle
- source_scope: risk-factor paragraphs on concurrent listing requirements, trading-market differences, data/privacy regimes, and AI-law developments

final_prompt_text:
Use the official company filing as anchor and one corroborating source if available. For dual-listed technology company regulatory-risk disclosure, resolve concurrent listing requirements and AI-law risk context.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish listing requirements from operating regulation, concurrent compliance from duplicated shares, AI-law risk from general data-privacy risk, and disclosed risk factor from an actual enforcement finding. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 8. BND-CORE-PAIR-044

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: acute public-health event detection and verification system
answer_unit: annual signal, risk-assessment, and public-reporting volume

source_anchor:
- Health-emergency report text says hundreds of signals were detected annually and followed up with requests for verification.
- It says 290 events annually on average were risk assessed and nearly 300 bulletins, announcements, or reports were shared annually with member states and the public.

internal_source_boundary:
- source_name: internal health-emergency surveillance source bundle
- source_scope: foreword/summary paragraphs on signal detection, verification requests, risk assessments, and public reporting volumes

final_prompt_text:
Use the official health-emergency report as anchor and one corroborating source if available. For acute public-health event detection and verification system, resolve annual signal, risk-assessment, and public-reporting volume.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish detected signals from confirmed events, verification requests from risk assessments, public bulletins from member-state notifications, and annual averages from a single outbreak year. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 9. BND-CORE-PAIR-038

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: federal open-data governance model in Germany
answer_unit: hybrid governance rationale and federal-level limitation

source_anchor:
- Country response text says the governance model is hybrid because of federal structures.
- It says the national government cannot directly mandate federal states or communes/cities to maintain a data inventory.

internal_source_boundary:
- source_name: internal open-data country-response source bundle
- source_scope: Germany response paragraphs on hybrid open-data governance, federal structures, and limitation on mandating state or municipal data inventories

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For federal open-data governance model in Germany, resolve hybrid governance rationale and federal-level limitation.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish hybrid governance from centralised governance, federal-state autonomy from national portal coordination, data inventory obligation from voluntary dataset publication, and regional high-value-dataset planning from nationwide implementation. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 10. BND-CORE-PAIR-034

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: EU adult lifestyle-risk disparities in 2022
answer_unit: education gap in daily smoking and adult heavy-drinking prevalence

source_anchor:
- Health-system report text says daily smoking in 2022 had a 14 percentage-point difference between adults with low and high levels of education.
- It says one in five adults reported heavy alcohol consumption on a monthly basis.

internal_source_boundary:
- source_name: internal health-system report source bundle
- source_scope: executive-summary paragraph on lifestyle risk factors, daily smoking education gap, and monthly heavy alcohol consumption

final_prompt_text:
Use the official health-system report as anchor and one corroborating source if available. For EU adult lifestyle-risk disparities in 2022, resolve education gap in daily smoking and adult heavy-drinking prevalence.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish adult smoking from adolescent risk behaviours, education gap from overall prevalence, monthly heavy drinking from daily alcohol use, and 2022 survey reference from later health-policy targets. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 11. CORE-TECH-13

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: foundation-model fine-tuning in federated learning frameworks
answer_unit: framework support status and remaining non-IID/privacy/communication challenge

source_anchor:
- Technical survey text says multiple federated-learning frameworks have adopted recent advancements and especially allow parameter-efficient fine-tuning of foundation models.
- It says key remaining challenges include efficient training, communication efficiency, non-IID data effects, and the interplay between fine-tuning and privacy.

internal_source_boundary:
- source_name: internal federated-learning survey source bundle
- source_scope: paragraphs on foundation models, parameter-efficient fine-tuning, supported frameworks, communication load, non-IID data, and privacy interaction

final_prompt_text:
Use the primary technical survey as anchor and one corroborating source if available. For foundation-model fine-tuning in federated learning frameworks, resolve framework support status and remaining non-IID/privacy/communication challenge.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish support for fine-tuning from efficient large-scale training, parameter-efficient adapters from full-model updates, non-IID data effects from privacy leakage, and survey claim from benchmarked framework performance. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 12. CORE-SCI-01

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: AI-readiness strategy for education systems
answer_unit: infrastructure, human-capacity, public-good, and ethical-risk components

source_anchor:
- Education technology text says preparing for an AI-driven future requires a comprehensive strategy focused on infrastructure, human capacity building, public-good creation, and ethical governance.
- It also says countries must diagnose readiness and tailor AI solutions rather than banning or ignoring AI.

internal_source_boundary:
- source_name: internal education-technology policy source bundle
- source_scope: conclusion and strategy paragraphs on AI readiness, infrastructure, human capacity, public-good creation, and ethical risk management

final_prompt_text:
Use the official education-policy source as anchor and one corroborating source if available. For AI-readiness strategy for education systems, resolve infrastructure, human-capacity, public-good, and ethical-risk components.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish readiness diagnosis from technology procurement, public-good creation from private tool adoption, ethical-risk governance from generic digital skills, and policy recommendation from evidence of implementation. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 13. CORE-POL-11

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Cyprus open-data governance board in 2024
answer_unit: stakeholder composition and purpose of the new governance body

source_anchor:
- Country factsheet text says a new Open Data Governance Board will bring together government bodies, private-sector entities, academia, and civil society.
- It says the board is intended to foster a collaborative approach to open-data initiatives.

internal_source_boundary:
- source_name: internal open-data maturity country-factsheet source bundle
- source_scope: Cyprus factsheet paragraph on the new governance board, stakeholder groups, and collaborative open-data initiatives

final_prompt_text:
Use the official country factsheet as anchor and one corroborating source if available. For Cyprus open-data governance board in 2024, resolve stakeholder composition and purpose of the new governance body.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish governance-board composition from portal maturity score, stakeholder inclusion from statutory decision power, collaborative initiative support from measured reuse impact, and 2024 factsheet status from future institutional changes. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 14. CORE-TECH-18

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: energy-efficiency policy toolkit implementation safeguards
answer_unit: monitoring-and-evaluation requirement and policy-update logic

source_anchor:
- Policy toolkit text says programmes should be periodically evaluated, ideally by independent researchers.
- It says evaluation should be transparent and include objectives, indicators, and methods, with amendments based on lessons learned from implementation.

internal_source_boundary:
- source_name: internal energy-efficiency policy-toolkit source bundle
- source_scope: policy-design paragraphs on programme evaluation, transparency, objectives, indicators, methods, collaboration, and amendments after implementation

final_prompt_text:
Use the official policy toolkit as anchor and one corroborating source if available. For energy-efficiency policy toolkit implementation safeguards, resolve monitoring-and-evaluation requirement and policy-update logic.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish evaluation requirement from compliance enforcement, independent evaluation from internal reporting, policy amendments from initial design standards, and toolkit recommendation from binding national law. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 15. CORE-POL-27

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: open-data AI reuse cases in environmental supervision
answer_unit: road-class F1 score and agriculture-use precision claim

source_anchor:
- Country-response text says an AI use case produced an F1 score of 0.98794618 for specific road classes less likely to have major accidents and need intervention.
- It says agriculture-use precision is roughly 85%, reducing the need for public officials to conduct on-site inspections in most cases.

internal_source_boundary:
- source_name: internal open-data AI-reuse country-response source bundle
- source_scope: reuse-case paragraph on road-class F1 score, agriculture precision, inspection avoidance, and environmental supervision applications

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For open-data AI reuse cases in environmental supervision, resolve road-class F1 score and agriculture-use precision claim.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish F1 score from precision, road-class model from agriculture-use case, claimed inspection reduction from measured cost savings, and reuse-case self-report from independently validated model performance. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 16. CORE-POL-25

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: open-data reuse for health-service management
answer_unit: hospital-workload, medical-personnel, and equipment-availability data role

source_anchor:
- Country-response text says open data enables effective monitoring and management of health services.
- It gives the national health information system as an example providing data on hospital workload, availability of medical personnel, and equipment.

internal_source_boundary:
- source_name: internal open-data reuse country-response source bundle
- source_scope: paragraph on health-service management, hospital workload, medical personnel availability, equipment availability, and monitoring role

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For open-data reuse for health-service management, resolve hospital-workload, medical-personnel, and equipment-availability data role.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish data availability from real-time operational control, health-service monitoring from patient-level clinical data, equipment availability from procurement spending, and reuse-case description from quantified health outcomes. Return: concise conclusion, source comparison, caveat, and confidence.
