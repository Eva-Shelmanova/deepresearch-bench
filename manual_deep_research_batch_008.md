# Manual Deep-Research Prompt Batch 008

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

## 1. CORE-ECON-03

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: generative-AI system inventory controls
answer_unit: inventory exemption rule and record-retention practice

source_anchor:
- Risk-management appendix text says organisations should define inventory exemptions for generative-AI systems embedded into application software.
- It also says organisations should maintain a document retention policy for test, evaluation, validation, verification, and digital-content transparency records.

internal_source_boundary:
- source_name: internal generative-AI risk-management source bundle
- source_scope: governance and information-security control rows on AI system inventory exemptions and document retention

final_prompt_text:
Use the controlling framework source as anchor and one corroborating source if available. For generative-AI system inventory controls, resolve the inventory exemption rule and record-retention practice.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish inventory exemptions from inventory absence, embedded application components from standalone systems, document retention from incident disclosure, and framework controls from binding legal duties. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 2. CORE-GEN-06

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: trust-survey implementation wave
answer_unit: 2023 fieldwork timing and participating-country count compared with 2021

source_anchor:
- Survey methodology text says the 2023 wave was implemented in 30 countries in October and November 2023.
- It says the inaugural 2021 wave included 22 countries.

internal_source_boundary:
- source_name: internal public-trust survey methodology source bundle
- source_scope: methodology paragraph on 2023 survey fieldwork timing, participating-country count, and 2021 comparison

final_prompt_text:
Use the official survey methodology source as anchor and one corroborating source if available. For trust-survey implementation wave, resolve 2023 fieldwork timing and participating-country count compared with 2021.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish fieldwork period from publication date, participating countries from member countries, survey wave count from respondent count, and 2023 expansion from changes in question wording. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 3. CORE-POL-08

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: law-enforcement data-transfer guideline adoption
answer_unit: adoption date and legal article addressed

source_anchor:
- Data-protection annual-report text says Guidelines 01/2023 on Article 37 of the Law Enforcement Directive were adopted on 19 June 2024.
- It says the guidelines address cross-border data transfers by law-enforcement authorities.

internal_source_boundary:
- source_name: internal data-protection annual-report source bundle
- source_scope: guidelines section on Article 37 of the Law Enforcement Directive, adoption date, and transfer scope

final_prompt_text:
Use the official data-protection source as anchor and one corroborating source if available. For law-enforcement data-transfer guideline adoption, resolve adoption date and legal article addressed.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish adoption date from publication or application date, guideline number from legal article, law-enforcement transfers from general data transfers, and guideline status from binding court ruling. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 4. CORE-POL-14

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Germany open-data reuse and impact controls in 2024
answer_unit: reuse-definition status, reuse-monitoring status, and impact-measurement methodology status

source_anchor:
- Country factsheet text records "Yes" for having a definition of open-data reuse.
- It records "Yes" for processes to monitor reuse and "Yes" for having a methodology to measure impact.

internal_source_boundary:
- source_name: internal open-data maturity country-factsheet source bundle
- source_scope: Germany factsheet key-question rows on reuse definition, reuse monitoring, and impact-measurement methodology

final_prompt_text:
Use the official country factsheet as anchor and one corroborating source if available. For Germany open-data reuse and impact controls in 2024, resolve reuse-definition status, reuse-monitoring status, and impact-measurement methodology status.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish reuse definition from reuse examples, monitoring processes from measured outcomes, impact methodology from overall maturity score, and country-specific answers from neighbouring factsheets. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 5. CORE-POL-20

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Romania open-data governance bodies in 2024
answer_unit: newly established governance bodies and coordination role

source_anchor:
- Country factsheet text says new governance bodies were established in 2024.
- It names a national coordination committee on data, digital services and AI, and a technical group for data-driven public-sector development.
- It says governance is anchored by central government and digitalisation authorities that coordinate input from public administrations, reusers, academia, and civil society.

internal_source_boundary:
- source_name: internal open-data maturity country-factsheet source bundle
- source_scope: Romania factsheet paragraph on 2024 governance bodies, coordinating authorities, and stakeholder input

final_prompt_text:
Use the official country factsheet as anchor and one corroborating source if available. For Romania open-data governance bodies in 2024, resolve newly established governance bodies and coordination role.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish newly established bodies from pre-existing coordinating authorities, data governance from portal scoring, stakeholder input from formal membership, and 2024 factsheet status from later institutional changes. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 6. CORE-POL-23

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: Ukraine open-data training initiative in 2024
answer_unit: training initiative purpose and target audience

source_anchor:
- Country factsheet text says the Open Data Academy was launched in 2024.
- It describes a cycle of educational training sessions for specialists driving digital transformation at the local level.
- It says the initiative aims to raise competencies of regional civil servants in open data.

internal_source_boundary:
- source_name: internal open-data maturity country-factsheet source bundle
- source_scope: Ukraine factsheet paragraph on 2024 Open Data Academy launch, local digital-transformation specialists, and civil-servant competencies

final_prompt_text:
Use the official country factsheet as anchor and one corroborating source if available. For Ukraine open-data training initiative in 2024, resolve training initiative purpose and target audience.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish academy launch from national portal functionality, local digital-transformation specialists from all civil servants, competency building from dataset publication, and 2024 initiative status from long-term programme outcomes. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 7. CORE-POL-30

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: national open-data impact strategy update
answer_unit: impact theme in the 2023-2027 strategy and publisher-pillar commitments

source_anchor:
- Country response text says the 2017-2022 strategy included a theme on evaluating impact, benefits and risks.
- It says the 2023-2027 strategy describes open-data benefits and impact, and that the publisher pillar includes goals for standard formats, relevant data publication, and timely upload frequency.

internal_source_boundary:
- source_name: internal open-data strategy country-response source bundle
- source_scope: strategy paragraphs on impact theme, publisher pillar, standard formats, relevant datasets, and upload frequency

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For national open-data impact strategy update, resolve impact theme in the 2023-2027 strategy and publisher-pillar commitments.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish strategic commitments from measured implementation, impact theme from impact methodology, publisher-pillar goals from user-pillar goals, and 2017-2022 strategy language from 2023-2027 updates. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 8. CORE-POL-31

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: demand-driven open-data conversion practice
answer_unit: provider-interview scale and conversion of single-indicator requests

source_anchor:
- Country response text says approximately 300 in-depth interviews with potential data providers had been conducted.
- It says the state data agency developed a practice of converting individual single-indicator requests into universal demand-driven open datasets.

internal_source_boundary:
- source_name: internal open-data demand-management country-response source bundle
- source_scope: paragraph on provider interviews, demand-driven collections, and conversion of single-indicator requests into open datasets

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For demand-driven open-data conversion practice, resolve provider-interview scale and conversion of single-indicator requests.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish potential data-provider interviews from user interviews, single-indicator requests from bulk dataset publication, universal open datasets from restricted sensitive-data access, and reported practice from legally mandated process. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 9. CORE-POL-34

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: 2024 open-data impact survey expansion
answer_unit: respondent groups added to the survey

source_anchor:
- Country response text says a 2024 edition of the survey on open-data impact is being conducted among open-data officers.
- It says the survey is expanded to representatives of cities that have open-data portals.

internal_source_boundary:
- source_name: internal open-data impact survey country-response source bundle
- source_scope: paragraph on 2024 survey edition, open-data officers, city representatives, and portal-user questionnaire reports

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For 2024 open-data impact survey expansion, resolve respondent groups added to the survey.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish open-data officers from city representatives, 2024 survey expansion from earlier survey reports, impact survey respondents from portal users, and planned or ongoing survey work from published results. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 10. CORE-POL-37

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: open-data portal reuse examples update
answer_unit: beta-section status and timing of reuse-example visibility

source_anchor:
- Country response text says a new section with good examples was added in March 2024.
- It notes that the feature was in beta and that a clear reuse-case page was expected later.

internal_source_boundary:
- source_name: internal open-data portal country-response source bundle
- source_scope: country response rows on beta good-examples section, reuse-case page plans, and filtering statistics

final_prompt_text:
Use the official country response as anchor and one corroborating source if available. For open-data portal reuse examples update, resolve beta-section status and timing of reuse-example visibility.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish beta feature from fully released page, good examples from formal reuse-case registry, March 2024 launch from future filtering functionality, and portal visibility from measured reuse impact. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 11. CORE-SCI-05

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: women in technology education and access indicators
answer_unit: STEM graduate share, science-engineering-ICT job share, and connectivity gaps

source_anchor:
- Gender-and-technology text says women make up only 35% of STEM graduates.
- It says women hold only a quarter of science, engineering and ICT jobs.
- It also reports 130 million fewer women than men own a mobile phone and 244 million fewer women have internet access worldwide.

internal_source_boundary:
- source_name: internal gender-and-technology source bundle
- source_scope: paragraph on STEM graduates, science/engineering/ICT job share, mobile-phone ownership gap, and internet-access gap

final_prompt_text:
Use the official analytical source as anchor and one corroborating source if available. For women in technology education and access indicators, resolve STEM graduate share, science-engineering-ICT job share, and connectivity gaps.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish graduates from workforce jobs, science-engineering-ICT jobs from all technology jobs, absolute access gaps from percentages, and global indicators from regional or income-group estimates. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 12. CORE-SCI-08

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: learning-poverty indicator definition
answer_unit: age threshold and reading-comprehension standard

source_anchor:
- Learning-poverty brief says the indicator focuses on the share of children who do not learn to read with comprehension by age 10.
- It also says that in low- and middle-income countries, more than half of children cannot read and understand a short age-appropriate text by the end of primary school.

internal_source_boundary:
- source_name: internal learning-poverty brief source bundle
- source_scope: introductory paragraphs defining learning poverty, age threshold, and short age-appropriate text standard

final_prompt_text:
Use the official indicator brief as anchor and one corroborating source if available. For learning-poverty indicator definition, resolve age threshold and reading-comprehension standard.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish learning poverty from school attendance, age 10 from end-of-primary timing, short age-appropriate text from any literacy task, and low- and middle-income country context from a single-country estimate. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 13. CORE-SCI-15

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: labour-force survey methodology revision
answer_unit: data-collection and employment-status question changes

source_anchor:
- Methodology text says a labour-force survey regulation introduced important changes.
- It lists general use of computer-aided interviews and changes to the formulation of questions related to employment status during the reference week.

internal_source_boundary:
- source_name: internal labour-force survey methodology source bundle
- source_scope: methodology note on regulation-driven survey changes, data collection, and employment-status question formulation

final_prompt_text:
Use the official methodology source as anchor and one corroborating source if available. For labour-force survey methodology revision, resolve data-collection and employment-status question changes.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish data-collection mode from sampling frame, question wording from classification definitions, reference-week employment from annual labour status, and methodology change from observed labour-market change. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 14. CORE-TECH-07

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: digital-government policy framework dimensions
answer_unit: number of dimensions and role of digital-by-design

source_anchor:
- Digital-government text says the policy framework establishes six dimensions critical for digital government.
- It defines "digital by design" as designing policies to enable coherent public-sector use of digital tools and data when formulating policy.

internal_source_boundary:
- source_name: internal digital-government policy source bundle
- source_scope: framework paragraph listing six dimensions and defining digital-by-design

final_prompt_text:
Use the official policy framework source as anchor and one corroborating source if available. For digital-government policy framework dimensions, resolve number of dimensions and role of digital-by-design.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish framework dimensions from policy priorities, digital-by-design from digital-only service delivery, public-sector tool use from private-sector adoption, and framework definition from country implementation score. Return: current classification with boundary note, source comparison, caveat, and confidence.

---

## 15. BND-CORE-PAIR-003

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: beverage company euro-denominated note issuance
answer_unit: May 2024 initial principal amount and outstanding amount at year-end

source_anchor:
- Annual-report text says notes were issued in May 2024 in an aggregate initial principal amount of EUR 500,000,000.
- It says the same amount was outstanding as of the reporting date.

internal_source_boundary:
- source_name: internal company annual-report source bundle
- source_scope: debt note paragraph on May 2024 euro-denominated issuance, initial principal amount, and outstanding amount

final_prompt_text:
Use the official company report as anchor and one corroborating source if available. For beverage company euro-denominated note issuance, resolve May 2024 initial principal amount and outstanding amount at year-end.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish initial principal from fair value or carrying value, euro-denominated amount from dollar translation, issued amount from outstanding amount, and note issuance from unfunded investment commitments. Return: best-supported estimate or range, source comparison, caveat, and confidence.

---

## 16. BND-CORE-PAIR-029

task_type: open_web_multi_source_uncertainty_research
manual_status: ready
research_object: debt-advice service return-on-investment assumption
answer_unit: employable advice-seeker share and assumed job-loss avoidance share

source_anchor:
- Debt-advice report text says a 2017 estimate considered publicly funded debt-advice services across four benefit characteristics.
- For the first characteristic, it says that of the 20% employable advice seekers, 25% would have experienced job loss without social debt advice.

internal_source_boundary:
- source_name: internal debt-advice evaluation source bundle
- source_scope: return-on-investment paragraph on employable advice seekers and job-loss avoidance assumption

final_prompt_text:
Use the primary evaluation source as anchor and one corroborating source if available. For debt-advice service return-on-investment assumption, resolve employable advice-seeker share and assumed job-loss avoidance share.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish employable advice seekers from all advice seekers, assumed avoided job loss from observed employment outcome, one benefit characteristic from total return on investment, and 2017 estimate from later service-delivery evidence. Return: best-supported estimate or range, source comparison, caveat, and confidence.
