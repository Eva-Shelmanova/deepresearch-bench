# Manual Deep-Research Prompt Batch 012

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

## 1. CORE-ECON-16

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: emerging-market job-growth pressure from demographic expansion
answer_unit: expected working-age population growth and job-creation implication

source_anchor:
- Global economic text says working-age population expansion in many lower-income economies is large relative to previous rapid-expansion episodes.
- It says almost all economies in the relevant region are expected to face average annual working-age population growth that exceeds recent job growth, intensifying the need for employment creation.

internal_source_boundary:
- source_name: internal global-economic outlook source bundle
- source_scope: paragraphs on demographic expansion, working-age population growth, subdued job growth, and employment pressure in emerging and developing economies

final_prompt_text:
Use the official global economic outlook as anchor and one corroborating source if available. For emerging-market job-growth pressure from demographic expansion, resolve expected working-age population growth and job-creation implication.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish working-age population growth from total population growth, job growth from labour-force participation, regional pattern from every country, and forecast implication from observed employment outcomes. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 2. BND-CORE-PAIR-048

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: accessibility-complaints open-data reuse case
answer_unit: complaint-data publication and related dataset-search boundary

source_anchor:
- Country-response text points to data about digital-accessibility complaints.
- It also distinguishes a complaints dataset from a broader search over accessibility-related datasets on the national portal.

internal_source_boundary:
- source_name: internal open-data reuse country-response source bundle
- source_scope: paragraph on digital-accessibility complaint data, complaints dataset link, and broader accessibility dataset search

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For accessibility-complaints open-data reuse case, resolve complaint-data publication and related dataset-search boundary.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish a complaint-history dataset from all accessibility datasets, publication of complaints from resolution of complaints, reuse evidence from portal search results, and accessibility policy from open-data availability. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 3. BND-CORE-PAIR-022

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: labour-market tightness and real-wage recovery
answer_unit: unemployment-rate reference point and real-wage recovery caveat

source_anchor:
- Employment-outlook text says the United States unemployment rate was 4.1 percent in June 2024, still near historic lows despite a small increase over the previous year.
- It says real wages are growing year-on-year in most countries but remain below their 2019 level in many countries.

internal_source_boundary:
- source_name: internal employment-outlook source bundle
- source_scope: labour-market summary paragraphs on unemployment, labour-market tightness, real-wage growth, and remaining gap from 2019

final_prompt_text:
Use the official labour-market outlook as anchor and one corroborating source if available. For labour-market tightness and real-wage recovery, resolve unemployment-rate reference point and real-wage recovery caveat.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish one country's unemployment reference point from cross-country labour-market tightness, nominal from real wages, year-on-year wage growth from recovery to 2019 levels, and current labour-market status from net-zero transition analysis. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 4. BND-CORE-PAIR-049

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: transport-data reuse outreach in 2024
answer_unit: target user groups and event-based engagement evidence

source_anchor:
- Country-response text says individual reusers include universities, large and small businesses, and citizens.
- It says two user groups were engaged through a poster at a leading data-science conference in February 2024 and through related events.

internal_source_boundary:
- source_name: internal open-data reuse country-response source bundle
- source_scope: paragraphs on transport-data reusers, university/business/citizen groups, and February 2024 event engagement

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For transport-data reuse outreach in 2024, resolve target user groups and event-based engagement evidence.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish outreach evidence from measured reuse impact, transport-data users from all portal users, event participation from formal consultation, and 2024 engagement from standing governance arrangements. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 5. BND-CORE-PAIR-002

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: global-bank 2024 organizational simplification
answer_unit: completion timing and management-structure purpose

source_anchor:
- Annual-report text says the bank completed its organizational simplification during the first quarter of 2024 after announcing it in September 2023.
- It says the result was a simpler management structure aligned with strategy and intended to improve accountability.

internal_source_boundary:
- source_name: internal bank annual-report source bundle
- source_scope: executive-summary paragraph on organizational simplification, first-quarter 2024 completion, September 2023 announcement, and accountability purpose

final_prompt_text:
Use the official company report as anchor and one corroborating source if available. For global-bank 2024 organizational simplification, resolve completion timing and management-structure purpose.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish completion of structural simplification from broader strategy execution, announcement date from completion quarter, management accountability from financial performance, and organizational change from product or client-service launches. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 6. CORE-TECH-14

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: retrieval-augmented generation versus long-context models
answer_unit: reported benchmark improvement and later efficiency-comparison caveat

source_anchor:
- Technical survey text says one retrieval-tree method paired with a frontier model improved accuracy on a long-form reasoning benchmark by 20 percent.
- It also says later research compared retrieval-augmented generation with long-context language models, making the relative efficiency question more method-dependent.

internal_source_boundary:
- source_name: internal retrieval-augmented generation survey source bundle
- source_scope: survey paragraphs on retrieval-tree method, benchmark improvement, long-context model comparison, and current limitations

final_prompt_text:
Use the primary technical survey as anchor and one corroborating source if available. For retrieval-augmented generation versus long-context models, resolve reported benchmark improvement and later efficiency-comparison caveat.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish accuracy improvement from efficiency improvement, one benchmark result from general superiority, retrieval method from long-context baseline, and survey summary from original experimental evidence. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 7. CORE-POL-43

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: open-data policy dimension maturity in Europe
answer_unit: average policy-dimension score, year-to-year change, and high-value dataset requirement

source_anchor:
- Regional maturity report text says the policy dimension remained the most mature dimension on average at 91 percent, with a 2 percentage-point increase since 2023.
- It says high-value dataset categories should be made available free of charge, in machine-readable formats, through APIs and, where relevant, as bulk downloads.

internal_source_boundary:
- source_name: internal regional open-data maturity report source bundle
- source_scope: policy-dimension paragraphs on average score, change since 2023, high-value datasets, free access, machine-readable formats, APIs, and bulk download

final_prompt_text:
Use the official regional maturity report as anchor and one corroborating source if available. For open-data policy dimension maturity in Europe, resolve average policy-dimension score, year-to-year change, and high-value dataset requirement.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish policy-dimension maturity from overall maturity, percentage-point change from percent change, high-value dataset obligations from all datasets, and policy framework score from actual reuse outcomes. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 8. CORE-ECON-02

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: post-tightening financial-sector resilience
answer_unit: banking-turmoil assessment and remaining vulnerability warning

source_anchor:
- Financial-stability text says bank failures in Switzerland and the United States in March 2023 did not lead to broader ruptures and that major emerging markets remained resilient through the interest-rate upswing.
- It also warns that vulnerabilities are mounting and policymakers should act to limit fragilities.

internal_source_boundary:
- source_name: internal financial-stability outlook source bundle
- source_scope: paragraphs on March 2023 bank failures, emerging-market resilience, interest-rate upswing, contained risks, and mounting vulnerabilities

final_prompt_text:
Use the official financial-stability outlook as anchor and one corroborating source if available. For post-tightening financial-sector resilience, resolve banking-turmoil assessment and remaining vulnerability warning.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish contained financial stress from absence of vulnerability, emerging-market resilience from advanced-economy bank failures, monetary-tightening effects from fiscal risks, and current assessment from forward-looking warning. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 9. CORE-POL-28

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: national open-data leadership reorganisation in France
answer_unit: leadership shift and ministerial-roadmap update

source_anchor:
- Country-response text says open-data policy is no longer led by the previous unit after a reorganisation and is now led by the national portal team within an interministerial product operator.
- It says new ministerial roadmaps on data, algorithms, and source-code policy were to be adopted by the end of 2023.

internal_source_boundary:
- source_name: internal open-data country-response source bundle
- source_scope: France response paragraphs on reorganisation, open-data policy leadership, national portal team, product operator, and ministerial roadmaps

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For national open-data leadership reorganisation in France, resolve leadership shift and ministerial-roadmap update.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish policy leadership from portal operation, organisational reallocation from repeal of open-data policy, planned roadmaps from adopted legal obligations, and national data policy from regional dataset publication. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 10. BND-CORE-PAIR-039

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: national data portal high-value dataset tagging in Sweden
answer_unit: legal basis, inventory responsibility, and incomplete tagging status

source_anchor:
- Country-response text says the digital-government agency is responsible for holding the national open-data inventory through the national data portal.
- It says the possibility to denote and follow high-value datasets exists in the portal, but all relevant datasets have not yet been denoted and this remains up to each data producer.

internal_source_boundary:
- source_name: internal open-data country-response source bundle
- source_scope: Sweden response paragraphs on legal basis, national open-data inventory, portal responsibility, high-value dataset denotation, and producer responsibility

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For national data portal high-value dataset tagging in Sweden, resolve legal basis, inventory responsibility, and incomplete tagging status.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish portal capability from complete implementation, national inventory responsibility from dataset-producer tagging, high-value dataset denotation from dataset publication, and current status from future compliance plans. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 11. BND-CORE-PAIR-016

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: product-recycling automation capability
answer_unit: device-model disassembly capacity and component-output count

source_anchor:
- Environmental progress text says a recycling robot can take apart 29 models of a smartphone product into 15 discrete components.
- It also says additional recycling machines are deployed with a recycling partner, and a new product sorter was introduced to improve efficiency.

internal_source_boundary:
- source_name: internal environmental-progress report source bundle
- source_scope: recycling-technology paragraph on disassembly models, component outputs, partner deployment, and product sorter introduction

final_prompt_text:
Use the official environmental progress report as anchor and one corroborating source if available. For product-recycling automation capability, resolve device-model disassembly capacity and component-output count.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish model count from unit volume, component categories from recovered material quantities, recycling-robot capability from actual recycling rate, and newly introduced sorter from previously deployed machines. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 12. BND-CORE-PAIR-008

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: low-income-country debt-vulnerability status
answer_unit: risk-of-debt-distress claim and recovery-since-pandemic caveat

source_anchor:
- Global economic text says elevated debt levels pose severe challenges in low-income countries, with not a single low-income country at low risk of debt distress.
- It also says recent recovery among emerging and developing economies remains insufficient to make up for lost ground since 2020, particularly in vulnerable economies.

internal_source_boundary:
- source_name: internal global-economic outlook source bundle
- source_scope: paragraphs on low-income-country debt distress, recovery since 2020, vulnerable economies, and fiscal-space constraints

final_prompt_text:
Use the official global economic outlook as anchor and one corroborating source if available. For low-income-country debt-vulnerability status, resolve risk-of-debt-distress claim and recovery-since-pandemic caveat.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish low-income countries from all emerging markets, debt distress risk from actual default, recovery in output from recovery in fiscal space, and forecast vulnerability from current debt classification. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 13. CORE-TECH-20

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: generative-AI system inventory governance
answer_unit: inventory exemptions and document-retention requirement

source_anchor:
- Risk-management profile text says organisations should define inventory exemptions for generative-AI systems embedded into application software.
- It also says organisations should maintain a document-retention policy to keep history for testing, evaluation, validation, verification, and digital-content transparency processes.

internal_source_boundary:
- source_name: internal AI risk-management profile source bundle
- source_scope: governance action rows on generative-AI system inventory exemptions and document retention for evaluation and transparency processes

final_prompt_text:
Use the official AI risk-management profile as anchor and one corroborating source if available. For generative-AI system inventory governance, resolve inventory exemptions and document-retention requirement.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish inventory exemption policy from exclusion of risk management, embedded systems from standalone models, document retention from public disclosure, and profile action from legally binding compliance duty. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 14. CORE-TECH-08

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: AI risk mapping and measurement functions
answer_unit: MAP-to-MEASURE relationship and ongoing risk-tracking requirement

source_anchor:
- Risk-management framework text says outcomes in the MAP function are the basis for MEASURE and MANAGE functions.
- It says mechanisms for tracking identified AI risks over time should be in place, with evaluation and documentation of testing, evaluation, validation, and verification metrics and processes.

internal_source_boundary:
- source_name: internal AI risk-management framework source bundle
- source_scope: framework paragraphs on MAP outcomes, MEASURE function, risk tracking over time, and evaluation/documentation of testing processes

final_prompt_text:
Use the official AI risk-management framework as anchor and one corroborating source if available. For AI risk mapping and measurement functions, resolve MAP-to-MEASURE relationship and ongoing risk-tracking requirement.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish mapping context from measuring risk, risk tracking from one-time testing, framework function from ordered checklist, and socio-technical risk awareness from purely technical model metrics. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 15. CORE-POL-44

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: governance-indicator margins of error
answer_unit: comparison caution and reform-evaluation limitation

source_anchor:
- Governance-indicator methodology text says margins of error are explicitly reported alongside estimates and should be considered when comparing governance estimates across countries.
- It says the indicators are not designed to evaluate specific governance reforms in individual economies and should be supplemented with more granular country-specific data for that purpose.

internal_source_boundary:
- source_name: internal governance-indicator methodology source bundle
- source_scope: methodology paragraphs on margins of error, cross-country comparison, perceptions, and limitations for reform evaluation

final_prompt_text:
Use the official governance-indicator methodology as anchor and one corroborating source if available. For governance-indicator margins of error, resolve comparison caution and reform-evaluation limitation.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish estimate from confidence interval, cross-country comparison from reform evaluation, perception-based source aggregation from objective administrative measurement, and aggregate indicator from granular country evidence. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 16. CORE-GEN-11

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: household cost-of-living pressure in well-being indicators
answer_unit: low-income housing-cost burden and post-inflation caveat

source_anchor:
- Well-being report text says in 2022 nearly one in five low-income households across covered countries spent over 40 percent of disposable income on housing costs.
- It says cost-of-living pressures may still be widespread despite income and employment shock mitigation, especially for vulnerable households.

internal_source_boundary:
- source_name: internal well-being indicators report source bundle
- source_scope: paragraphs on cost-of-living pressures, low-income household housing costs, disposable-income threshold, vulnerable households, and post-inflation assessment

final_prompt_text:
Use the official well-being indicators report as anchor and one corroborating source if available. For household cost-of-living pressure in well-being indicators, resolve low-income housing-cost burden and post-inflation caveat.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish low-income households from all households, housing-cost burden from general inflation, disposable income from gross income, and 2022 indicator value from later subjective financial-stress evidence. Return: best-supported estimate or range, source comparison, caveat, and confidence.
