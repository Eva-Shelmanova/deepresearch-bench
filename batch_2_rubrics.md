# Batch 2 Evaluation Artifacts

Evaluation artifacts for the 16 runnable tasks in `manual_deep_research_batch_002.md`.

Phase 10 rule:
- Core tasks use a task-level rubric with five fixed criteria: Coverage, Accuracy, Reasoning, Use of evidence, Clarity and structure.
- Each Core criterion is scored 0-2, for 10 total points.
- Set tasks use a gold set, not a narrative rubric. Set scoring is precision, recall, and F1 against the bounded gold set.

---

## 1. CORE-POL-39

rubric_id: CORE-RUBRIC-B02-CORE-POL-39
task_type: Core
research_object: countries driving global population growth to 2050
answer_unit: group of countries contributing more than half of projected global population increase through 2050

### Key Facts From Source Bundle

- A small group of countries is projected to contribute more than half of global population growth through 2050.
- The group is **Democratic Republic of the Congo, Egypt, Ethiopia, India, Nigeria, Pakistan, the Philippines, and Tanzania**.
- The claim is a demographic projection, not observed historical growth.
- The relevant horizon is through **2050**.
- Projection variant, fertility, mortality, migration, and later revisions affect interpretation.
- The group is not simply the world's largest-population countries.

### Expected Response Sections

- Conclusion naming the projected country group.
- Source comparison with the official demographic projection as anchor.
- Boundary explanation about projection horizon, variant, and grouping.
- Caveat about projection assumptions and possible later revisions.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Names the full group and covers horizon, projection status, comparison, caveat, and confidence.
- 1: Names most countries but omits a required section or relevant boundary.
- 0: Does not identify the projected group.

**Accuracy**
- 2: Gives all eight countries correctly.
- 1: Omits or adds one country while preserving the general claim.
- 0: Gives a different group or replaces the answer with largest-population countries.

**Reasoning**
- 2: Distinguishes projection from observed growth and explains time horizon, grouping, and variant assumptions.
- 1: Mentions projection or horizon but leaves assumptions unclear.
- 0: Treats the claim as observed growth or ignores the projection boundary.

**Use of Evidence**
- 2: Anchors in the official demographic projection and uses another source only to check wording, variant, or revision status.
- 1: Uses one source with limited explanation or compares sources without variant awareness.
- 0: Relies on generic population rankings or unsupported search results.

**Clarity and Structure**
- 2: Gives a concise list plus comparison, caveat, and confidence.
- 1: Understandable but cluttered or missing one expected section.
- 0: Broad demographic essay without the requested group.

### Common Failure Modes

- Omitting one of the eight countries.
- Adding populous countries not in the stated group.
- Treating the projection as already observed growth.
- Ignoring fertility, mortality, migration, or projection-variant caveats.

### Borderline Cases

- Minor naming variants such as "DR Congo" are acceptable.
- Ordering does not matter unless the response invents a ranking not supported by the source.
- If a later projection revision differs, the answer should explain the source vintage rather than silently replacing the original group.

---

## 2. BND-CORE-PAIR-018

rubric_id: CORE-RUBRIC-B02-BND-CORE-PAIR-018
task_type: Core
research_object: France inflation forecast
answer_unit: forecast inflation rates for 2024 and 2025

### Key Facts From Source Bundle

- The task asks for France's forecast inflation rates.
- The expected rates are **2.3% for 2024** and **2.0% for 2025**.
- The measure is headline inflation unless the controlling source specifies otherwise.
- The values are forecasts, not later actuals.
- Forecast vintage matters.
- Annual-average forecasts must not be confused with monthly point-in-time inflation.

### Expected Response Sections

- Conclusion with both forecast rates.
- Source comparison checking measure and forecast vintage.
- Boundary explanation about headline/core/harmonised inflation and annual versus monthly measures.
- Caveat about revisions, later actuals, and source vintage.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Reports both years and includes measure, forecast status, comparison, caveat, and confidence.
- 1: Reports both rates but omits one or two required sections.
- 0: Does not answer both forecast years.

**Accuracy**
- 2: Gives **2.3% for 2024** and **2.0% for 2025**.
- 1: Gives one correct rate or gives close values with unclear measure/vintage.
- 0: Gives euro-area rates, later actuals, or unrelated inflation values.

**Reasoning**
- 2: Distinguishes headline/core/harmonised measures, forecast vintage, annual average, and later actuals.
- 1: Mentions one boundary but leaves another important one unclear.
- 0: Mixes measures or treats later data as the original forecast.

**Use of Evidence**
- 2: Uses the official macro outlook as anchor and compares only measure-compatible sources.
- 1: Uses a source comparison but does not fully align measure or date.
- 0: Uses unsupported values or incompatible inflation series.

**Clarity and Structure**
- 2: Clearly states both year-value pairs and the caveat/confidence.
- 1: Understandable but not well structured.
- 0: Hard to parse or mostly about inflation generally.

### Common Failure Modes

- Reporting euro-area inflation instead of France.
- Mixing headline, core, and harmonised measures without saying so.
- Treating revised actual data as the original forecast.
- Omitting one of the two years.

### Borderline Cases

- Accept "around 2.3%" and "around 2.0%" if the source comparison and forecast vintage are clear.
- Do not penalize a later-source note if the answer preserves the requested forecast.
- If using HICP, the answer must say whether it is the same measure used by the controlling source.

---

## 3. CORE-POL-09

rubric_id: CORE-RUBRIC-B02-CORE-POL-09
task_type: Core
research_object: Albania open-data legal implementation
answer_unit: entry-into-force date of the open-data law

### Key Facts From Source Bundle

- The law is Albania's Law No. 33/2022 on Open Data and Reuse of Public Sector Information.
- The entry-into-force date is **29 April 2023**.
- Entry into force is distinct from enactment, publication, transposition, and implementation deadline.
- Legal force does not prove that every reusable dataset was practically available.
- Official legal or public-administration sources are controlling for the date.

### Expected Response Sections

- Conclusion with the entry-into-force date.
- Source comparison using official legal/public-administration evidence.
- Boundary explanation separating enactment, publication, entry into force, and implementation.
- Caveat about practical data availability or later legal updates.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes date, law identity, legal boundary, source comparison, caveat, and confidence.
- 1: Gives date and law but omits comparison or caveat.
- 0: Does not answer the entry-into-force question.

**Accuracy**
- 2: Gives **29 April 2023** as the entry-into-force date.
- 1: Gives April 2023 or a nearby date with partial support.
- 0: Gives the law number, enactment date, or publication date as the effective date.

**Reasoning**
- 2: Clearly distinguishes enactment, publication, legal entry into force, implementation deadline, and practical availability.
- 1: Mentions a legal distinction but leaves the specific date type unclear.
- 0: Conflates legal force with implementation or publication.

**Use of Evidence**
- 2: Anchors in an official legal/public-administration source and uses corroboration to check date/category consistency.
- 1: Uses one official source with limited explanation.
- 0: Relies on secondary summaries without date-type verification.

**Clarity and Structure**
- 2: Concise legal/status conclusion with comparison, caveat, and confidence.
- 1: Understandable but includes unnecessary legal summary.
- 0: Broad open-data discussion without the date.

### Common Failure Modes

- Giving the 2022 law number as the effective date.
- Confusing entry into force with implementation deadline.
- Reporting a transposition or publication date without checking effective date.
- Assuming legal force means all reusable data were already available.

### Borderline Cases

- A response can receive partial credit if it gives the correct date but calls it "implementation" imprecisely.
- Do not require a long legal summary; over-explaining should not compensate for a wrong date.
- If the response notes later amendments, it must keep the original entry-into-force answer distinct.

---

## 4. CORE-POL-21

rubric_id: CORE-RUBRIC-B02-CORE-POL-21
task_type: Core
research_object: Slovenia dynamic public-sector data reuse
answer_unit: immediate reuse rule for dynamic data after collection

### Key Facts From Source Bundle

- Slovenia's open-data reform includes immediate reuse of dynamic data after collection.
- The answer concerns dynamic data, not all public-sector datasets.
- Immediate reuse is a legal/policy rule, not proof of real-time technical API availability.
- Implementation can depend on technical feasibility, data categories, and exceptions.
- Official legal or reform sources are controlling.

### Expected Response Sections

- Conclusion stating the immediate reuse rule for dynamic data.
- Source comparison anchored in official legal/reform evidence.
- Boundary explanation about dynamic versus static data and legal permission versus operational access.
- Caveat about implementation limits, technical feasibility, or exceptions.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Covers immediate reuse, dynamic-data scope, legal/technical boundary, evidence, caveat, and confidence.
- 1: States the rule but omits an important boundary or evidence section.
- 0: Does not identify the dynamic-data rule.

**Accuracy**
- 2: Correctly states that dynamic data should be reusable immediately after collection.
- 1: States a similar rule but with unclear data scope or timing.
- 0: Says all public-sector information is immediately reusable or gives another rule.

**Reasoning**
- 2: Distinguishes dynamic/static data, legal reuse permission, API/real-time access, and practical implementation.
- 1: Mentions one distinction but does not explain its consequence.
- 0: Equates legal reuse with guaranteed real-time access.

**Use of Evidence**
- 2: Uses official legal/reform evidence as anchor and corroborates boundary or implementation status.
- 1: Uses one relevant source with limited comparison.
- 0: Uses general open-data principles without source-specific support.

**Clarity and Structure**
- 2: Focused conclusion with clear boundary, caveat, and confidence.
- 1: Mostly clear but overly broad.
- 0: Broad open-data essay or unclear answer.

### Common Failure Modes

- Saying all public-sector data are immediately reusable.
- Treating "dynamic" as simply "recently updated."
- Equating legal reuse with guaranteed real-time API delivery.
- Ignoring exceptions or practical implementation limits.

### Borderline Cases

- Partial credit is appropriate if the answer says "near-real-time" but explains that the legal rule is immediate reuse after collection.
- Do not penalize lack of technical implementation detail if the response explicitly caveats it as beyond the legal rule.
- If a source uses translated wording, accept close equivalents for "dynamic data."

---

## 5. CORE-TECH-02

rubric_id: CORE-RUBRIC-B02-CORE-TECH-02
task_type: Core
research_object: EU technical support instrument budget
answer_unit: EUR 864 million budget

### Key Facts From Source Bundle

- The technical-support instrument budget is **EUR 864 million**.
- The budget supports Member State structural reforms.
- The amount is a programme envelope, not necessarily annual payments or project-level spending.
- Currency and price convention must be preserved where available.
- The instrument is distinct from broader EU digital or recovery funding programmes.

### Expected Response Sections

- Conclusion with EUR 864 million.
- Source comparison using the official programme/budget source as anchor.
- Boundary explanation about programme envelope, payments, commitments, and reform scope.
- Caveat about price convention, period, or budget implementation.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes amount, currency, programme scope, evidence, caveat, and confidence.
- 1: Gives amount but omits scope or budget-boundary detail.
- 0: Does not identify the EUR 864 million budget.

**Accuracy**
- 2: Reports **EUR 864 million** for the technical-support instrument.
- 1: Reports a close value or the right programme but incomplete currency/amount context.
- 0: Reports another EU programme budget or wrong amount.

**Reasoning**
- 2: Distinguishes envelope, annual commitments, payments, current-price convention, and eligible reform scope.
- 1: Mentions programme scope but leaves budget convention unclear.
- 0: Treats the amount as annual spending or project-level expenditure without support.

**Use of Evidence**
- 2: Anchors in an official EU/programme source and checks consistency with a compatible source.
- 1: Uses one relevant source or compares sources without budget-convention alignment.
- 0: Uses unrelated EU funding figures or unsupported summaries.

**Clarity and Structure**
- 2: Concise amount and scope statement with caveat and confidence.
- 1: Understandable but includes unnecessary EU funding background.
- 0: Unclear or mostly unrelated to the instrument.

### Common Failure Modes

- Reporting a different EU programme budget.
- Treating EUR 864 million as an annual amount when the source gives a programme envelope.
- Omitting the eligible structural-reform context.
- Mixing commitments, allocations, and payments.

### Borderline Cases

- If the response gives EUR 864m without price-period detail, it can still earn partial accuracy but not full coverage/reasoning.
- Accept "€864 million" as equivalent.
- Do not reward broader EU budget numbers unless the requested instrument is clearly isolated.

---

## 6. CORE-ECON-13

rubric_id: CORE-RUBRIC-B02-CORE-ECON-13
task_type: Core
research_object: OECD unemployment rate in May 2024
answer_unit: unemployment rate around May 2024

### Key Facts From Source Bundle

- The unemployment rate across the country group was **4.9%** by/around May 2024.
- The rate is an area-wide or country-group rate, not a single national rate.
- The reference month is around **May 2024**.
- Seasonal adjustment and population coverage may matter if specified by the source.
- Later revisions or later months should be caveated.

### Expected Response Sections

- Conclusion with the unemployment rate and reference month.
- Source comparison using official labour-market evidence.
- Boundary explanation about area-wide versus national rate, reference month, and adjustment.
- Caveat about coverage and later revisions.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Gives rate, month, country-group scope, evidence, caveat, and confidence.
- 1: Gives the rate but omits reference month, scope, or caveat.
- 0: Does not answer the unemployment-rate question.

**Accuracy**
- 2: Reports **4.9% around May 2024** for the country group.
- 1: Reports a close value or right rate with unclear month/scope.
- 0: Reports a single-country rate or a different labour-market measure.

**Reasoning**
- 2: Distinguishes harmonised area-wide rate, national rates, seasonally adjusted/unadjusted data, reference month, and population coverage.
- 1: Mentions scope or month but not both clearly.
- 0: Mixes employment, labour force, and unemployment measures.

**Use of Evidence**
- 2: Anchors in the official labour-market source and corroborates with compatible data or update notes.
- 1: Uses one source with limited explanation.
- 0: Uses unsupported values or incompatible national data.

**Clarity and Structure**
- 2: Clear numeric answer with comparison, caveat, and confidence.
- 1: Understandable but not well structured.
- 0: Unclear or focused on unrelated labour-market discussion.

### Common Failure Modes

- Reporting a single country's unemployment rate.
- Using a later month without noting the update/revision.
- Mixing labour force, employment, and unemployment measures.
- Omitting whether the rate applies to the country group.

### Borderline Cases

- "About 5%" can earn partial accuracy if scope and month are correct.
- If a later release gives a revised May value, the answer should identify the revision rather than silently replacing the source-bundle value.
- Do not penalize missing seasonal-adjustment detail if the source does not specify it, but reward answers that check it.

---

## 7. CORE-ECON-07

rubric_id: CORE-RUBRIC-B02-CORE-ECON-07
task_type: Core
research_object: industrial company dividend and connected-machine target
answer_unit: EUR 1.15 dividend proposal and 80% by 2030 target distinction

### Key Facts From Source Bundle

- The proposed 2024 dividend is **EUR 1.15 per share**.
- The proposed dividend is up **15 cents** from the previous year.
- The company target is to connect **80% of enabled installed machines** for digital applications by **2030**.
- The dividend proposal is distinct from an approved or paid dividend.
- The 80% target denominator is enabled installed machines, not all machines.
- The financial-return metric and digital-machine target are separate answer components.

### Expected Response Sections

- Conclusion with both the dividend proposal and the connected-machine target.
- Source comparison using official company/performance evidence.
- Boundary explanation about proposed versus paid dividend and target denominator.
- Caveat about approval/payment status and target scope.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes both answer components, relevant years, denominator, comparison, caveat, and confidence.
- 1: Includes one component fully and the other partially, or omits caveat/comparison.
- 0: Omits one answer component entirely.

**Accuracy**
- 2: Reports **EUR 1.15 per share** proposed 2024 dividend and **80% of enabled installed machines by 2030**.
- 1: Gives one correct figure and one incomplete or slightly ambiguous figure.
- 0: Gives wrong figures or merges the two metrics.

**Reasoning**
- 2: Separates proposed/approved/paid dividend and enabled-machine target denominator from broader installed-base counts.
- 1: Mentions one distinction but not the other.
- 0: Conflates financial-return and digital-machine metrics.

**Use of Evidence**
- 2: Anchors in official company reporting and uses corroboration only to check proposal/status or target wording.
- 1: Uses a relevant source but with limited comparison.
- 0: Uses unsupported company summaries or unrelated financial data.

**Clarity and Structure**
- 2: Clearly presents two separate answer components with caveat and confidence.
- 1: Mostly understandable but the two components are not cleanly separated.
- 0: Confusing or mostly unrelated to the requested metrics.

### Common Failure Modes

- Treating the dividend as already paid.
- Reporting 80% of all machines instead of enabled installed machines.
- Confusing 2030 target timing with 2024 dividend year.
- Omitting one of the two answer components.

### Borderline Cases

- Missing the 15-cent increase should not block full accuracy if the two required answer components are correct.
- If the dividend was later approved, the answer must preserve that the source-bundle answer unit is the proposal and caveat the update.
- Accept "€1.15" as equivalent to EUR 1.15.

---

## 8. CORE-POL-42

rubric_id: CORE-RUBRIC-B02-CORE-POL-42
task_type: Core
research_object: public-sector data release exclusion rule
answer_unit: confidentiality, sensitivity, or lack-of-control limit on releasability

### Key Facts From Source Bundle

- Some public-sector information cannot be released as open data.
- Reasons include confidentiality, sensitivity, third-party or control limits, and lack of full administrative control.
- These are legal/policy exclusions, not failures of portal quality.
- The rule limits releasability even when general open-data policy encourages release.
- The answer should not imply unconditional publication of all public-sector information.

### Expected Response Sections

- Conclusion explaining the exclusion rule.
- Source comparison using official legal/policy evidence.
- Boundary explanation distinguishing exclusions from open-data goals.
- Caveat about legal category, third-party rights, or administrative-control limits.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes confidentiality/sensitivity, lack-of-control or third-party limits, evidence, caveat, and confidence.
- 1: Includes some exclusion reasons but omits one required boundary or section.
- 0: Does not explain releasability limits.

**Accuracy**
- 2: Correctly states that confidential, sensitive, or not-fully-controlled information may be excluded from open-data release.
- 1: Gives a partial exclusion rule but omits a central category.
- 0: Says all public-sector information must be released or gives an unrelated rule.

**Reasoning**
- 2: Distinguishes legal exclusions from policy goals, portal quality, and general open-government rhetoric.
- 1: Mentions exclusions but does not explain why they limit releasability.
- 0: Treats open-data policy as unconditional release.

**Use of Evidence**
- 2: Anchors in official reuse/open-data evidence and uses corroboration to clarify legal or policy boundary.
- 1: Uses one relevant source with limited comparison.
- 0: Relies on generic open-data claims.

**Clarity and Structure**
- 2: Clear concise rule with boundary, caveat, and confidence.
- 1: Understandable but broad.
- 0: Unfocused open-government essay.

### Common Failure Modes

- Treating open-data policy as unconditional release.
- Ignoring third-party rights or administrative-control limits.
- Confusing non-release with poor portal quality.
- Answering with a broad open-government essay.

### Borderline Cases

- A response can earn high accuracy if it uses equivalent terms such as "restricted", "protected", or "not under the administration's control."
- Do not require all possible legal exceptions if the central confidentiality/sensitivity/control boundary is correct.
- If a source mentions personal data, evaluate it under confidentiality/sensitivity unless it replaces the broader rule incorrectly.

---

## 9. CORE-TECH-16

rubric_id: CORE-RUBRIC-B02-CORE-TECH-16
task_type: Core
research_object: cybersecurity incident-reporting simplification
answer_unit: single cybersecurity incident-reporting mechanism

### Key Facts From Source Bundle

- A digital simplification proposal includes a **single mechanism** for related cybersecurity incident-reporting obligations.
- The status may be proposed rather than adopted.
- A reporting mechanism/channel is distinct from the underlying incident categories.
- The mechanism does not necessarily collapse all cybersecurity regimes into one obligation.
- Affected entities and legal scope matter if specified by the source.

### Expected Response Sections

- Conclusion on the single incident-reporting mechanism.
- Source comparison checking proposal/adoption status.
- Boundary explanation about mechanism versus obligations, categories, and affected entities.
- Caveat about legal status and implementation.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Covers mechanism, status, scope, source comparison, caveat, and confidence.
- 1: Covers the mechanism but omits status or scope.
- 0: Does not identify the single reporting mechanism.

**Accuracy**
- 2: Correctly states that the proposal includes a single mechanism for related cybersecurity incident-reporting obligations.
- 1: Gives a partially correct description with unclear legal status or scope.
- 0: Claims all cybersecurity obligations are merged or gives a wrong mechanism.

**Reasoning**
- 2: Distinguishes proposal/adoption, reporting channel, incident categories, affected entities, and underlying legal duties.
- 1: Mentions proposed status or mechanism but does not fully separate concepts.
- 0: Conflates incident reporting with incident prevention, monitoring, or all cybersecurity law.

**Use of Evidence**
- 2: Anchors in the official simplification source and corroborates legal status or scope.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic cybersecurity commentary or unsupported status claims.

**Clarity and Structure**
- 2: Focused conclusion with source comparison, caveat, and confidence.
- 1: Understandable but vague on status.
- 0: Unclear or unrelated cybersecurity discussion.

### Common Failure Modes

- Presenting the mechanism as already fully in force without checking status.
- Ignoring which reporting obligations are being simplified.
- Confusing incident reporting with incident prevention or monitoring.
- Overgeneralising to all cybersecurity incidents.

### Borderline Cases

- If the answer says "single entry point" or "single reporting channel," accept it if it matches the mechanism boundary.
- Do not require exhaustive legal article citations if status and scope are correctly handled.
- If adoption status changed later, the answer should explain the update against the original proposal context.

---

## 10. CORE-POL-38

rubric_id: CORE-RUBRIC-B02-CORE-POL-38
task_type: Core
research_object: family migration and care-worker dependants
answer_unit: 373,000 family migrants in 2023 and March 2024 dependant rule change

### Key Facts From Source Bundle

- Family migration reached **373,000** in **2023**.
- This was a **60% increase from 2022**.
- From **March 2024**, new care workers under the relevant visa route can no longer bring family members.
- Family migrants and care-worker dependants are related but not identical categories.
- Grants, applications, arrivals, dependants, route categories, and reporting years must be kept separate.
- Later policy updates or source-definition changes should be caveated.

### Expected Response Sections

- Conclusion with the 2023 family-migration number, 60% increase, and March 2024 rule change.
- Source comparison using official migration/policy evidence.
- Boundary explanation separating migration categories, grants/applications/arrivals, and visa-route scope.
- Caveat about definitions, reporting year, and later policy updates.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes all three key answer components plus category boundary, evidence, caveat, and confidence.
- 1: Includes two key components or omits important boundary/caveat detail.
- 0: Omits the migration number or the rule change.

**Accuracy**
- 2: Reports **373,000 family migrants in 2023**, **60% increase from 2022**, and **March 2024** care-worker dependant restriction.
- 1: Gets two of the three components correct or gives one with minor ambiguity.
- 0: Gives wrong numbers/timing or applies the rule to the wrong visa category.

**Reasoning**
- 2: Distinguishes grants/applications/arrivals/dependants, route-specific rules, and reporting-year boundaries.
- 1: Mentions categories but does not fully separate them.
- 0: Treats family migrants and care-worker dependants as the same category.

**Use of Evidence**
- 2: Anchors in official migration/policy evidence and corroborates definitions or update status.
- 1: Uses one relevant source or compares sources without aligning definitions.
- 0: Uses unsupported migration commentary or incompatible categories.

**Clarity and Structure**
- 2: Clearly separates number, increase, rule change, caveat, and confidence.
- 1: Mostly understandable but combines categories confusingly.
- 0: Unclear or broad migration-policy essay.

### Common Failure Modes

- Treating family migrants and care-worker dependants as the same category.
- Using applications instead of migrants/grants.
- Omitting the 60% increase or the March 2024 timing.
- Applying the dependant restriction to all visa routes.

### Borderline Cases

- If "family migrants" is reported as "family visas/grants," partial credit depends on whether the source definition supports that wording.
- Do not require all visa-route details if the route-specific care-worker restriction is clear.
- A later policy update should not erase the requested 2023/2024 answer components.

---

## 11. SET-GEN-F04

gold_set_id: SET-GOLD-B02-SET-GEN-F04
task_type: Set
research_object: United States nominal GDP row
candidate_item: United States
answer_unit: leading nominal GDP estimate recorded for the candidate

### Correct Items

- Candidate row: **United States**.
- Required measure: **nominal GDP** / GDP at current prices / current US-dollar GDP.
- Required value: the **United States row's leading nominal GDP estimate** in the controlling table at lookup time.
- Required metadata: table year or estimate year, unit, and source convention.

### Acceptable Variants

- "United States", "U.S.", "USA", or "United States of America" if tied to the same row.
- Rounded values matching the source's displayed units.
- "Current-price GDP" or "GDP, current US$" if equivalent to nominal GDP.
- Estimate/forecast/observed wording if it follows the source convention.

### Optional Distractors

- China nominal GDP.
- United States PPP GDP.
- United States GDP per capita.
- United States real GDP or GDP growth.
- A full country ranking.

### Explicit Exclusion Rules

- Exclude PPP, real, constant-price, per-capita, and growth-rate values.
- Exclude values for countries other than the United States.
- Exclude mixed-year answers that do not preserve the controlling table year.
- Exclude whole-list retrieval.

### Boundary Notes

- The gold value can update; scoring should be against the controlling table row and lookup-time source convention.
- Precision/recall/F1 should use the bounded fields: row, measure, value, year/unit, and source convention.

---

## 12. BND-SET-SET005

gold_set_id: SET-GOLD-B02-BND-SET-SET005
task_type: Set
research_object: Australia sovereign-state row
candidate_item: Australia - Commonwealth of Australia
answer_unit: sovereignty/status category recorded for the candidate

### Correct Items

- Candidate row: **Australia / Commonwealth of Australia**.
- Correct status category: the controlling row's sovereignty or membership/status category, typically **sovereign state** and/or **UN member state** depending on the table convention.
- Required metadata: row naming convention and category wording used by the source.

### Acceptable Variants

- "Australia" and "Commonwealth of Australia" as equivalent row names.
- "Sovereign state", "independent sovereign state", or "UN member state" if matching the table's category convention.
- Explanatory note that "Commonwealth" is part of the formal name and does not imply non-sovereign status.

### Optional Distractors

- Continent/region: Oceania.
- Commonwealth realm.
- Federation.
- Dependent territory.
- Full sovereign-state list.

### Explicit Exclusion Rules

- Exclude answers that classify Australia as non-sovereign because of "Commonwealth" wording.
- Exclude geography-only answers.
- Exclude answers that report government form rather than sovereignty/status category unless the source category asks for it.
- Exclude full-list retrieval.

### Boundary Notes

- The gold set is bounded to the Australia row and its status/category field.
- Corroborating sources may confirm naming/status but should not override the controlling row wording without explicit evaluator update.

---

## 13. BND-SET-SET008

gold_set_id: SET-GOLD-B02-BND-SET-SET008
task_type: Set
research_object: Banjul International Airport code row
candidate_item: Banjul International Airport
answer_unit: IATA code recorded for the candidate

### Correct Items

- Candidate row: **Banjul International Airport**.
- Correct IATA code: **BJL**.
- Required distinction: IATA code, not ICAO code.
- Required metadata where available: current/former airport name and serving area if relevant to row matching.

### Acceptable Variants

- "Banjul International Airport" with former or alternate naming if linked to the same airport.
- "BJL" as the IATA airport code.
- A note that the ICAO code is different, if used only as a boundary check.

### Optional Distractors

- ICAO code.
- Banjul city without airport row.
- Former-name entry not tied to the current airport.
- Full airport-code list.

### Explicit Exclusion Rules

- Exclude ICAO code answers as the requested answer unit.
- Exclude city-only answers.
- Exclude outdated or alternative names unless they are clearly mapped to the same airport row.
- Exclude whole-list retrieval.

### Boundary Notes

- Precision/recall/F1 should treat **BJL** as the required item and airport-row matching as a required boundary condition.
- Secondary airport lists may corroborate but the aviation-code row/register is controlling.

---

## 14. SET-TECH-E03

gold_set_id: SET-GOLD-B02-SET-TECH-E03
task_type: Set
research_object: SQL programming-language boundary entry
candidate_item: SQL
answer_unit: language category used to justify inclusion of the candidate

### Correct Items

- Candidate item: **SQL**.
- Correct category: **query language** and/or **domain-specific language** included under the source's programming-language boundary.
- Required boundary: SQL is not being treated as an unqualified general-purpose language and is not a database product.

### Acceptable Variants

- "Structured Query Language" as the expanded name.
- "Domain-specific programming language" if the source uses programming-language inclusion wording.
- "Database query language" if it preserves the source boundary.
- Notes about SQL dialects/families if they do not replace the core category.

### Optional Distractors

- Database management system.
- Markup language.
- General-purpose programming language without qualification.
- SQL dialect list.
- Full programming-language list.

### Explicit Exclusion Rules

- Exclude answers saying SQL is not included without addressing the source boundary.
- Exclude answers treating SQL as a database product.
- Exclude markup-only classifications.
- Exclude full-list retrieval.

### Boundary Notes

- Scoring should reward correct category and boundary reasoning, not a philosophical answer about whether SQL "really" is a programming language.
- Precision/recall/F1 should use the category fields: SQL, query/domain-specific language, inclusion boundary.

---

## 15. SET-GEN-F05

gold_set_id: SET-GOLD-B02-SET-GEN-F05
task_type: Set
research_object: Australia literacy-rate row
candidate_item: Australia
answer_unit: adult literacy-rate value recorded for the candidate

### Correct Items

- Candidate row: **Australia**.
- Required measure: **adult literacy rate**.
- Required value: the adult literacy-rate value recorded for Australia in the controlling table at lookup time, commonly around **99%** if that is the table value.
- Required metadata: estimate year, unit, and any missing-value or compilation note.

### Acceptable Variants

- "Australia" as country/economy row.
- Rounded literacy-rate values if they match the source's displayed rounding.
- "Adult literacy", "literacy rate, adult total", or equivalent source wording.
- Notes that the figure is estimated/compiled if the source says so.

### Optional Distractors

- Youth literacy rate.
- Education attainment or school enrollment.
- Reading-proficiency scores.
- A full literacy-rate list.
- Territory/economy rows other than Australia.

### Explicit Exclusion Rules

- Exclude youth literacy, education attainment, enrollment, or proficiency metrics.
- Exclude values without source year/unit when those are available in the row.
- Exclude answers that treat estimated/compiled values as direct census measurement without support.
- Exclude whole-list retrieval.

### Boundary Notes

- The gold value may vary by source year; stable scoring requires fixing the controlling table version or accepting source-consistent lookup-time values.
- Precision/recall/F1 should use the fields: candidate row, adult-literacy measure, value, year/unit, and source note.

---

## 16. SET-SCI-E01

gold_set_id: SET-GOLD-B02-SET-SCI-E01
task_type: Set
research_object: CHEA accreditation-organisation entry
candidate_item: Council for Higher Education Accreditation
answer_unit: accreditation-organisation category recorded for the candidate

### Correct Items

- Candidate item: **Council for Higher Education Accreditation** / **CHEA**.
- Correct answer unit: the source's recorded **accreditation-organisation category** for the candidate.
- Required distinction: organisation category, not accreditation status of a university.
- Required metadata: whether the category is a registry row, regional heading, or secondary compilation label.

### Acceptable Variants

- "CHEA" or full organisational name.
- Category wording that preserves the source meaning, such as accreditation organisation / higher-education accreditation organisation, if that matches the row.
- Notes distinguishing CHEA's institutional role from government-agency status.

### Optional Distractors

- Government accreditor.
- University accreditation status.
- Regional heading only.
- Full accreditation-organisation list.
- U.S. Department of Education recognition status used as the category without support from the controlling row.

### Explicit Exclusion Rules

- Exclude answers that report only the full name and not the category.
- Exclude answers classifying CHEA as a government agency without source support.
- Exclude university-level accreditation statuses.
- Exclude full-list retrieval.

### Boundary Notes

- The gold set is bounded to the CHEA row and the category field surrounding that row.
- Corroborating sources may clarify CHEA's role but should not override the controlling row category unless the evaluator updates the gold set.
