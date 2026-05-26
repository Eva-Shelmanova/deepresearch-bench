# Batch 1 Evaluation Artifacts

Evaluation artifacts for the three runnable tasks in `manual_prompt_rewrite_batch_001.md`.

Phase 10 rule:
- Core tasks use a task-level rubric with five fixed criteria: Coverage, Accuracy, Reasoning, Use of evidence, Clarity and structure.
- Each Core criterion is scored 0-2, for 10 total points.
- Set tasks use a gold set, not a narrative rubric. Set scoring is precision, recall, and F1 against the bounded gold set.

---

## 1. CORE-POL-01

rubric_id: CORE-RUBRIC-B01-CORE-POL-01
task_type: Core
research_object: Poland's new fiscal oversight body
answer_unit: planned operational start date

### Key Facts From Source Bundle

- Poland's new fiscal oversight body is the Fiscal Council / fiscal council body.
- The planned operational start date is **1 January 2026**.
- The date concerns when the body is expected to begin operations.
- The operational start is distinct from legal establishment, appointment, setup, or adoption milestones.
- The date is also distinct from the fiscal year or broader EU fiscal-governance reform dates.
- Later legal or implementation updates may affect whether the planned date remains current.

### Expected Response Sections

- Conclusion with the planned operational start date.
- Source comparison using an official primary source as anchor and at least one corroborating source where available.
- Boundary explanation separating operational start from other legal/setup dates.
- Caveat about planned/future status and possible updates.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Covers the date, institution, operational-start meaning, source comparison, caveat, and confidence.
- 1: Covers the date and institution but omits one or two required sections.
- 0: Does not cover the operational-start question.

**Accuracy**
- 2: Gives **1 January 2026** as the planned operational start date.
- 1: Gives 2026 or January 2026 but not the exact day, or gives the date with minor ambiguity.
- 0: Gives another date or treats the body as already operational without qualification.

**Reasoning**
- 2: Clearly separates operational start from establishment, appointment/setup, budget-year applicability, and reform adoption.
- 1: Mentions a relevant distinction but leaves the date category partly unclear.
- 0: Conflates operational start with legal enactment, appointment, or EU fiscal-governance reform timing.

**Use of Evidence**
- 2: Anchors the answer in an official source and uses another source to check date consistency, institutional naming, or later updates.
- 1: Uses one controlling official source with limited comparison, or compares sources without explaining why one is controlling.
- 0: Relies on unsupported snippets, generic background, or misattributes the date.

**Clarity and Structure**
- 2: Presents conclusion, comparison, caveat, and confidence in a concise structure.
- 1: Understandable but missing one expected section or includes distracting background.
- 0: Hard to parse or mostly unrelated to the operational start date.

### Common Failure Modes

- Answering when the law was adopted instead of when the body begins operations.
- Treating an appointment or setup milestone as the operational start.
- Using EU-wide fiscal-governance timing as Poland's start date.
- Naming the institution correctly but not resolving the date.

### Borderline Cases

- Award partial accuracy credit if the response says "January 2026" and otherwise handles the boundary correctly.
- Do not penalize use of "Fiscal Council" versus "fiscal oversight body" if the institution is clearly the same.
- A one-source answer can receive evidence credit only if it explains why the official source is controlling.

---

## 2. CORE-TECH-05

rubric_id: CORE-RUBRIC-B01-CORE-TECH-05
task_type: Core
research_object: enterprise software renewable-electricity disclosure link
answer_unit: whether the link is direct, indirect, or unsupported

### Key Facts From Source Bundle

- The task concerns an enterprise software company's renewable-electricity or emissions disclosure.
- The answer must classify the link as **direct**, **indirect**, or **unsupported**.
- Company-level electricity procurement or emissions accounting is not the same as system-level renewable-electricity transition outcomes.
- A direct link requires explicit evidence tying the company disclosure to direct procurement/consumption or direct transition impact.
- If the evidence only combines company sustainability reporting with broad energy-transition context, the best-supported classification is indirect or unsupported.
- Correlation, alignment, or contextual relevance is not enough to prove causal contribution.
- Scope, reporting period, accounting boundary, and causality are essential caveats.

### Expected Response Sections

- Conclusion explicitly choosing direct, indirect, or unsupported.
- Source comparison between company disclosure and system-level energy-transition evidence.
- Boundary explanation about company-level versus grid/economy-level evidence.
- Caveat about scope, period, accounting boundary, and causality.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes classification, company/system boundary, source comparison, causality caveat, and confidence.
- 1: Gives a classification but omits comparison, caveat, or confidence.
- 0: Discusses renewable electricity generally without answering the classification question.

**Accuracy**
- 2: Correctly classifies the relationship according to explicit evidence and avoids causal overclaim.
- 1: Gives a plausible classification but does not tie it clearly to the evidence.
- 0: Claims a direct causal link without support or fails to classify the link.

**Reasoning**
- 2: Explains why procurement/disclosure, emissions accounting, grid outcomes, and system transition evidence are different evidence layers.
- 1: Notes company versus system scope but does not explain its effect on the conclusion.
- 0: Treats company disclosure and system-level renewable progress as equivalent.

**Use of Evidence**
- 2: Uses the company disclosure as anchor where available and compares it with a relevant energy-transition source, explaining what each can prove.
- 1: Uses both evidence layers but only summarizes them, or uses one source with limited justification.
- 0: Uses unsupported claims, search snippets, or unrelated renewable-energy background.

**Clarity and Structure**
- 2: States "direct," "indirect," or "unsupported" clearly and keeps the answer focused.
- 1: The classification can be inferred but is not stated cleanly.
- 0: The response is an unfocused essay about renewable electricity.

### Common Failure Modes

- Assuming company renewable-energy purchasing proves direct system-level transition impact.
- Confusing emissions-reduction disclosure with renewable-electricity procurement.
- Treating broad clean-energy trends as company-specific corroboration.
- Failing to choose among direct, indirect, and unsupported.

### Borderline Cases

- If the answer says "indirect at most" and explains the evidence limit, score it as a valid classification.
- If the response finds an explicit direct procurement claim but not a system-level causal link, it should separate those two conclusions.
- Do not require a causal conclusion where the source bundle only supports disclosure or alignment.

---

## 3. SET-GEN-F04

gold_set_id: SET-GOLD-B01-SET-GEN-F04
task_type: Set
research_object: United States nominal GDP row
candidate_item: United States
answer_unit: leading nominal GDP estimate recorded for the candidate

### Correct Items

- Candidate row: **United States**.
- Required measure: **nominal GDP** / GDP at current prices / current US-dollar GDP, according to the controlling table convention.
- Required value: the **leading nominal GDP estimate recorded for the United States row** at lookup time.
- Required metadata: table year or estimate year, unit, and source convention.

### Acceptable Variants

- "United States", "U.S.", "USA", or "United States of America" if clearly tied to the same country/economy row.
- Rounded nominal GDP values if rounding matches the source's displayed units.
- "current-price GDP" or "GDP, current US$" if the value corresponds to nominal GDP.
- Estimate, forecast, or observed/current-price wording if it follows the source table's convention.

### Optional Distractors

- China nominal GDP.
- United States PPP GDP.
- United States GDP per capita.
- United States real GDP or constant-price GDP.
- United States GDP growth rate.
- A full country ranking copied from a table.

### Explicit Exclusion Rules

- Exclude PPP GDP, GDP per capita, real GDP, constant-price GDP, and growth-rate answers.
- Exclude values for countries other than the United States.
- Exclude answers that mix multiple source years without identifying the controlling table year.
- Exclude full-list retrieval as the answer unit; only the United States row is requested.

### Boundary Notes

- The gold value can change when live tables update, so scoring should use the controlling table row and lookup-time source convention.
- Precision/recall/F1 should be computed over the bounded fields: country row, nominal-GDP measure, value, year/unit, and source convention.
- Corroborating macroeconomic sources may check plausibility but should not override the controlling table row unless the evaluator intentionally updates the gold set.
# Batch 1 Rubrics

Rubrics for the three runnable tasks in `manual_prompt_rewrite_batch_001.md`.

Default scoring: 10 points per task. Award partial credit only for answers that directly address the named research object and answer unit. Do not reward broad essays, whole-list retrieval, or unsupported guesses.

For every task, the expected answer format is:
- conclusion
- source comparison
- caveat
- confidence level

---

## 1. CORE-POL-01

research_object: Poland's new fiscal oversight body
answer_unit: planned operational start date
task_type: open_web_multi_source_uncertainty_research

### Gold Expectation

The answer should conclude that Poland's new fiscal oversight body / Fiscal Council is planned to begin operations on **1 January 2026**, while distinguishing this operational start date from legal adoption, establishment, appointments, setup work, fiscal-year use, or broader EU fiscal-governance reform timing.

The answer should use an official fiscal-governance or Polish public-finance source as the anchor and use a corroborating source only to check date consistency, institutional naming, or later updates.

### Required Elements

- States the planned operational start date as **1 January 2026**.
- Identifies the body as Poland's fiscal oversight body / Fiscal Council without confusing it with another fiscal institution.
- Explains why the date refers to beginning operations, not merely legal establishment or board appointment.
- Compares at least two sources where available, or explains why one official source is controlling.
- Includes a caveat about planned/future status and possible later legal or implementation updates.
- Gives a confidence level.

### Scoring

**2 points - Correct conclusion**
- 2: Gives 1 January 2026 as the planned operational start date.
- 1: Gives 2026 or January 2026 but omits the exact day, or states the exact date with minor ambiguity.
- 0: Gives another date, treats the date as already operational without qualification, or does not answer the start-date question.

**2 points - Boundary and methodology**
- 2: Clearly separates operational start from legal establishment, appointments, setup milestones, and fiscal-year applicability.
- 1: Mentions one relevant distinction but leaves the date category partly unclear.
- 0: Conflates operational start with enactment, appointment, reform approval, or budget-year timing.

**2 points - Source comparison**
- 2: Uses an official primary source as anchor and checks consistency against another source or later update.
- 1: Uses only one source but explains that it is controlling, or uses two sources without meaningful comparison.
- 0: Does not identify source basis, relies on generic search snippets, or misattributes the date.

**2 points - Caveat and confidence**
- 2: Notes the planned/future nature of the date and gives a justified confidence level.
- 1: Gives either caveat or confidence, but not both, or gives a generic caveat.
- 0: Presents the answer as unconditional without uncertainty handling.

**2 points - Clarity**
- 2: Concise, structured answer with conclusion, comparison, caveat, and confidence.
- 1: Understandable but missing one requested section or includes distracting background.
- 0: Hard to parse, overly broad, or mostly unrelated to the operational start date.

### Common Failure Modes

- Answering when the law was adopted instead of when the body begins operations.
- Treating EU-wide fiscal-governance reform dates as Poland's operational date.
- Naming the institution correctly but not resolving the date.
- Overstating confidence without checking whether the date is still planned.

---

## 2. CORE-TECH-05

research_object: enterprise software renewable-electricity disclosure link
answer_unit: whether the link is direct, indirect, or unsupported
task_type: open_web_multi_source_uncertainty_research

### Gold Expectation

The answer should classify the link between an enterprise software company's renewable-electricity or emissions disclosure and broader renewable-electricity transition outcomes as **direct only if the company disclosure explicitly supports a direct procurement/consumption claim tied to renewable electricity**. If the source evidence only combines company-level sustainability reporting with system-level clean-electricity transition evidence, the best-supported conclusion should be **indirect or unsupported as a causal/system-level link**.

The answer must not infer that a company disclosure caused, materially drove, or directly explains a system-level renewable-electricity outcome unless the sources explicitly establish that relationship.

### Required Elements

- Classifies the link as direct, indirect, or unsupported.
- Distinguishes company-level electricity procurement/emissions disclosure from grid-level or economy-level renewable-electricity outcomes.
- Separates correlation, alignment, or contextual relevance from causal contribution.
- Uses the company disclosure as the anchor where available and compares it with system-level energy-transition evidence.
- Includes a caveat about scope, reporting period, measurement boundary, and causality.
- Gives a confidence level.

### Scoring

**2 points - Correct conclusion**
- 2: Correctly classifies the relationship as direct, indirect, or unsupported based on explicit source evidence, with no causal overclaim.
- 1: Gives a plausible classification but hedges unclearly or does not fully tie it to the evidence.
- 0: Claims a direct causal link without support, or does not classify the relationship.

**2 points - Boundary and methodology**
- 2: Clearly separates company-level disclosure, procurement, emissions accounting, grid outcomes, and system-level transition evidence.
- 1: Mentions company versus system scope but does not explain why it changes the conclusion.
- 0: Treats company disclosure and system-level renewable progress as the same evidence layer.

**2 points - Source comparison**
- 2: Compares the company source with at least one energy-transition/source-context source and explains what each can and cannot prove.
- 1: Uses both sources but only summarizes them, or uses one source with limited justification.
- 0: Uses one unsupported claim, a search snippet, or unrelated renewable-energy background.

**2 points - Caveat and confidence**
- 2: Gives a caveat about reporting scope, period, accounting boundary, and causality, plus justified confidence.
- 1: Gives a generic caveat or confidence without explaining the evidence limitation.
- 0: No caveat, no confidence, or unjustified certainty.

**2 points - Clarity**
- 2: The answer is compact and explicitly states "direct," "indirect," or "unsupported" in the conclusion.
- 1: The conclusion can be inferred but is not stated cleanly.
- 0: The response is an essay about renewable electricity without answering the classification question.

### Common Failure Modes

- Assuming renewable-energy purchasing by a company automatically implies a direct system-level transition impact.
- Confusing emissions-reduction disclosure with renewable-electricity procurement.
- Treating broad clean-energy trends as corroboration of a company-specific claim.
- Failing to choose among direct, indirect, and unsupported.

---

## 3. SET-GEN-F04

research_object: United States nominal GDP row
candidate_item: United States
answer_unit: leading nominal GDP estimate recorded for the candidate
task_type: online_multi_source_candidate_boundary_research

### Gold Expectation

The answer should retrieve the **leading nominal GDP estimate for the United States** from the relevant country/economy table row, preserving the table's year, unit, and source convention. The answer must not switch to PPP GDP, GDP per capita, constant-price GDP, real GDP growth, or a different year's value.

Because live GDP tables can update, grading should focus on whether the model correctly identifies the controlling table row, nominal-current-price measure, unit, source/year, and estimate as recorded at lookup time. A corroborating macroeconomic source may be used to check plausibility, but the primary table/register remains controlling for the requested row.

### Required Elements

- Reports the United States row's leading nominal GDP estimate.
- States the table year and unit, usually in current US dollars or equivalent table units.
- Identifies that the measure is nominal GDP, not PPP or real GDP.
- Explains whether the value is an estimate, forecast, or observed/current-price value according to the source table.
- Uses a corroborating source only to check plausibility or updated-year consistency.
- Includes a caveat about table updates, source-year differences, and rounding.
- Does not retrieve or reproduce the full GDP list.

### Scoring

**2 points - Correct value and row**
- 2: Gives the United States row's leading nominal GDP estimate with correct unit and table year.
- 1: Gives a close rounded value or correct row but incomplete year/unit.
- 0: Gives a PPP value, GDP per capita, real GDP growth, another country's value, or no estimate.

**2 points - Boundary and methodology**
- 2: Clearly separates nominal from PPP, current from constant prices, forecast/estimate from observed data, and table year from lookup date.
- 1: Mentions nominal GDP but leaves one major boundary unclear.
- 0: Conflates GDP concepts or ignores the table-year/source convention.

**2 points - Source comparison**
- 2: Uses the primary table/register as anchor and at least one corroborating source to check plausibility or update status.
- 1: Uses only the primary table but correctly explains it is controlling, or compares sources without addressing year/unit differences.
- 0: Uses a random search result, no source basis, or source comparison that changes the requested measure.

**2 points - Caveat and confidence**
- 2: Notes update/rounding/source-year caveats and gives a justified confidence level.
- 1: Gives only a generic caveat or confidence.
- 0: No caveat, no confidence, or misleading certainty despite possible table updates.

**2 points - Clarity and task discipline**
- 2: Directly answers the United States row question and does not retrieve the whole list.
- 1: Mostly answers but includes unnecessary list context or extra countries.
- 0: Provides a ranking/list instead of the candidate's answer unit, or the response is not focused on the United States row.

### Common Failure Modes

- Returning PPP GDP instead of nominal GDP.
- Reporting GDP growth, GDP per capita, or real GDP.
- Mixing values from different institutions without explaining year/unit differences.
- Copying a whole country ranking instead of the United States row.
- Omitting the table year or unit.
