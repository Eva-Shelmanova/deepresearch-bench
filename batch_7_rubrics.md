# Batch 7 Evaluation Artifacts

Evaluation artifacts for the 16 runnable tasks in `manual_deep_research_batch_007.md`.

Phase 10 rule:
- Core tasks use a task-level rubric with five fixed criteria: Coverage, Accuracy, Reasoning, Use of evidence, Clarity and structure.
- Each Core criterion is scored 0-2, for 10 total points.
- Batch 7 contains Core tasks only; no Set gold sets are required.

---

## 1. BND-CORE-PAIR-007

rubric_id: CORE-RUBRIC-B07-BND-CORE-PAIR-007
task_type: Core
research_object: large online retailer 2024 revenue growth
answer_unit: total revenue growth rate and starting/ending revenue values

### Key Facts From Source Bundle

- Total revenue grew **11% year over year**.
- Revenue increased from **$575B** to **$638B**.
- The answer concerns total revenue, not segment revenue.
- Year-over-year growth rate is distinct from absolute dollar increase.
- Fiscal-year reporting should be preserved over calendar-year headlines.
- Values are rounded billions unless exact reported figures are used.

### Expected Response Sections

- Conclusion with growth rate and starting/ending revenue values.
- Source comparison anchored in the official company report.
- Boundary explanation about total/segment revenue, growth rate/absolute change, fiscal/calendar year, and rounding.
- Caveat about rounded figures or exact reported values.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes growth rate, both revenue values, revenue scope, evidence, caveat, and confidence.
- 1: Gives growth rate and one value, or omits boundary/caveat detail.
- 0: Does not answer total revenue growth.

**Accuracy**
- 2: Reports **11%**, from **$575B** to **$638B**.
- 1: Gets two of the three numeric elements correct.
- 0: Reports segment revenue, operating income, cash flow, or incompatible values.

**Reasoning**
- 2: Distinguishes total/segment revenue, YoY rate/absolute increase, fiscal/calendar reporting, and rounded/exact figures.
- 1: Mentions one boundary but leaves another important one unclear.
- 0: Conflates revenue with other financial metrics or calculates a conflicting rate without caveat.

**Use of Evidence**
- 2: Uses the official company report and corroborates only compatible financial-reporting context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported market summaries or segment data as total revenue.

**Clarity and Structure**
- 2: Clear financial answer with source comparison, caveat, and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing financial summary.

### Common Failure Modes

- Reporting segment revenue instead of total revenue.
- Calculating a different percentage from rounded figures without caveat.
- Omitting either starting or ending revenue.
- Confusing revenue with operating income or cash flow.

### Borderline Cases

- Accept "$575 billion" and "$638 billion" as equivalent.
- If exact figures are used, they should reconcile with the rounded growth statement.
- Do not require identifying the retailer by name if the answer unit is correct.

---

## 2. BND-CORE-PAIR-023

rubric_id: CORE-RUBRIC-B07-BND-CORE-PAIR-023
task_type: Core
research_object: balance-of-payments assistance programme status in 2024
answer_unit: whether new operations or repayments occurred and expected programme end

### Key Facts From Source Bundle

- No new operations occurred in **2024**.
- No loan repayments occurred in **2024**.
- The programme is expected to end in **2025**.
- Expected end is linked to maturity of the outstanding loan and related borrowing.
- New operations are distinct from loan repayments.
- 2024 activity status is distinct from expected 2025 closure.
- The assistance line is distinct from other lending facilities.

### Expected Response Sections

- Conclusion with 2024 activity status and expected 2025 end.
- Source comparison anchored in the official financial report.
- Boundary explanation about operations/repayments, programme end/loan maturity, and other facilities.
- Caveat about expected rather than completed closure.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes no operations, no repayments, expected 2025 end, maturity reason, evidence, caveat, and confidence.
- 1: Includes activity status but omits end timing or maturity reason.
- 0: Does not answer programme status.

**Accuracy**
- 2: States **no new operations or repayments in 2024** and expected end in **2025** when outstanding loan/borrowing mature.
- 1: Gets activity status or expected end correct but not both.
- 0: Says repayments occurred in 2024 or closure was already completed.

**Reasoning**
- 2: Distinguishes operations/repayments, programme end/loan maturity, 2024 activity/2025 closure, and this assistance line/other facilities.
- 1: Mentions one distinction but leaves programme status unclear.
- 0: Conflates the programme with another lending facility.

**Use of Evidence**
- 2: Uses the official financial report and corroborates only compatible status/maturity details.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated assistance-programme summaries.

**Clarity and Structure**
- 2: Clear status conclusion with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing financial-programme answer.

### Common Failure Modes

- Saying repayments occurred in 2024.
- Treating expected 2025 closure as already completed.
- Confusing the programme with another assistance instrument.
- Omitting either the activity status or expected end.

### Borderline Cases

- Accept "no transactions" only if it clearly covers both new operations and repayments.
- Later maturity status should be caveated separately.
- Do not require detailed loan terms beyond maturity connection.

---

## 3. BND-CORE-PAIR-053

rubric_id: CORE-RUBRIC-B07-BND-CORE-PAIR-053
task_type: Core
research_object: Green Line crossings in 2024
answer_unit: direction of change in Greek Cypriot crossings compared with the previous year

### Key Facts From Source Bundle

- Greek Cypriot crossings decreased in **2024** compared with the previous year.
- The answer concerns Greek Cypriot crossings, not all crossings.
- Authorised crossing points are distinct from total mobility.
- The answer unit is direction of change, not an unsupported absolute count.
- The comparison is annual, not a longer-term trend.

### Expected Response Sections

- Conclusion with the direction of change.
- Source comparison anchored in the official implementation report.
- Boundary explanation about group scope, crossing points, annual comparison, and counts.
- Caveat about what the direction does and does not show.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes direction, group, year/comparison, evidence, caveat, and confidence.
- 1: Gives direction but omits group or comparison boundary.
- 0: Does not answer crossing direction.

**Accuracy**
- 2: States Greek Cypriot crossings **decreased in 2024 compared with the previous year**.
- 1: Says crossings decreased but does not specify Greek Cypriots.
- 0: Says crossings increased or reports unrelated mobility/migration data.

**Reasoning**
- 2: Distinguishes Greek Cypriot/other crossings, authorised crossing points/total mobility, direction/count, and annual/longer trend.
- 1: Mentions one boundary but leaves scope unclear.
- 0: Treats border-crossing changes as migration totals.

**Use of Evidence**
- 2: Uses the official implementation report and corroborates only compatible crossing-status information.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported absolute counts or unrelated border statistics.

**Clarity and Structure**
- 2: Direct direction-of-change answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Unclear border/mobility narrative.

### Common Failure Modes

- Reporting all crossings rather than Greek Cypriot crossings.
- Saying crossings increased.
- Inventing an absolute count not requested or not supported.
- Treating border-crossing changes as migration totals.

### Borderline Cases

- If the answer includes absolute counts, they must be sourced and not replace the direction answer.
- "Fell" and "declined" are equivalent to decreased.
- Do not require long-term trend analysis.

---

## 4. CORE-POL-07

rubric_id: CORE-RUBRIC-B07-CORE-POL-07
task_type: Core
research_object: internal audit recommendation follow-up at January 2025 cut-off
answer_unit: accepted recommendations assessed as effectively implemented

### Key Facts From Source Bundle

- The cut-off date is **31 January 2025**.
- The recommendation population is partially accepted recommendations made in **2020-2024**.
- **544 out of 831** were assessed by auditees as effectively implemented.
- The share is **65%**.
- Auditee-assessed implementation is distinct from independently verified closure.
- Partially accepted/accepted recommendations are distinct from all issued recommendations.

### Expected Response Sections

- Conclusion with numerator, denominator, share, population, and cut-off date.
- Source comparison anchored in the official audit report.
- Boundary explanation about recommendation population and auditee-assessed implementation.
- Caveat about independent verification/closure.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes cut-off, population, numerator, denominator, share, evidence, caveat, and confidence.
- 1: Includes share but omits numerator/denominator or population.
- 0: Does not answer implementation status.

**Accuracy**
- 2: Reports **544/831**, **65%**, as of **31 January 2025**, for **2020-2024** partially accepted recommendations.
- 1: Gets most numeric elements but omits one boundary.
- 0: Treats 65% as independent audit closure or applies it to wrong population.

**Reasoning**
- 2: Distinguishes accepted/issued, auditee-assessed/verified closure, partially/fully accepted, and population/cut-off.
- 1: Mentions one distinction but leaves implementation status unclear.
- 0: Conflates implementation assessment with final audit closure.

**Use of Evidence**
- 2: Uses official audit report evidence and corroborates only compatible follow-up status.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported audit-performance claims.

**Clarity and Structure**
- 2: Clear numeric status answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing audit follow-up answer.

### Common Failure Modes

- Treating 65% as independent audit closure.
- Omitting the 544/831 basis.
- Applying the figure to 2024 recommendations only.
- Confusing partially accepted and fully accepted recommendations.

### Borderline Cases

- If only 65% is given, accuracy is partial unless numerator/denominator appear elsewhere.
- Do not require audit-topic breakdowns.
- "Effectively implemented according to auditees" must not be upgraded to verified closure.

---

## 5. CORE-POL-40

rubric_id: CORE-RUBRIC-B07-CORE-POL-40
task_type: Core
research_object: genetically engineered crop adaptation-ratio example
answer_unit: adaptation ratio implied by yield-loss offset and baseline heat effect

### Key Facts From Source Bundle

- An additional hot day reduces yield by **0.293 units**.
- Genetically engineered varieties offset this yield loss by **0.0286 units**.
- The implied adaptation ratio is about **0.1**.
- The ratio is a coefficient ratio, not a percentage-point change.
- The offset does not fully eliminate the yield loss.
- The example concerns crop-yield adaptation, not general climate resilience.
- It is a study example, not a global average.

### Expected Response Sections

- Conclusion with yield-loss coefficient, offset coefficient, and adaptation ratio.
- Source comparison anchored in the primary analytical source.
- Boundary explanation about coefficient ratio, partial offset, and study/example scope.
- Caveat about generalisability.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes both coefficients, ratio, interpretation, evidence, caveat, and confidence.
- 1: Includes ratio but omits one coefficient or caveat.
- 0: Does not answer adaptation ratio.

**Accuracy**
- 2: Reports **0.293**, **0.0286**, and ratio about **0.1**.
- 1: Gets two numeric elements correct.
- 0: Reports 0.0286 as the ratio or says losses are fully offset.

**Reasoning**
- 2: Distinguishes coefficient ratio, percentage-point change, offset/full elimination, crop-yield adaptation/general resilience, and study example/global average.
- 1: Mentions one boundary but leaves ratio interpretation unclear.
- 0: Generalises the result to all crops/regions or treats 0.1 as unsupported yield gain.

**Use of Evidence**
- 2: Uses the primary analytical source and corroborates only compatible study-context details.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic climate adaptation claims.

**Clarity and Structure**
- 2: Clear coefficient-to-ratio explanation with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing adaptation calculation.

### Common Failure Modes

- Saying genetically engineered varieties fully offset heat losses.
- Reporting 0.0286 as the adaptation ratio.
- Treating 0.1 as a 10 percentage-point yield gain without explanation.
- Generalising the result to all crops or regions.

### Borderline Cases

- Accept "about one-tenth" for 0.1.
- Do not require recalculation if the source explicitly states the ratio and coefficients are correct.
- If the ratio is calculated as 0.0286/0.293, rounding differences are acceptable.

---

## 6. CORE-GEN-09

rubric_id: CORE-RUBRIC-B07-CORE-GEN-09
task_type: Core
research_object: China childlessness cohort-note definitions
answer_unit: birth cohorts and datasets used for reported China childlessness estimates

### Key Facts From Source Bundle

- China's **1935 cohort** refers to women born in **1931-1935**.
- China's **1955 cohort** refers to women born in **1951-1955**.
- These two cohorts were calculated using the **1995 dataset**.
- The **1970 cohort** used the **2015 dataset**.
- Cohort label is distinct from actual birth-year range.
- Dataset year is distinct from cohort year.
- The note concerns permanent childlessness, not fertility rate.
- The definitions are China-specific notes, not generic figure labels.

### Expected Response Sections

- Conclusion mapping cohort labels to birth ranges and dataset years.
- Source comparison anchored in the official statistical/social-indicator source.
- Boundary explanation about cohort labels, dataset years, permanent childlessness, and China-specific notes.
- Caveat about figure-note definitions.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes all cohort ranges, dataset mapping, definition boundaries, evidence, caveat, and confidence.
- 1: Includes most mappings but omits one cohort or dataset.
- 0: Does not answer cohort/dataset definitions.

**Accuracy**
- 2: Correctly maps 1935 to **1931-1935**, 1955 to **1951-1955**, both to **1995 dataset**, and 1970 to **2015 dataset**.
- 1: Gets most mappings but swaps or omits one element.
- 0: Treats cohort labels as single birth years or reports fertility rates.

**Reasoning**
- 2: Distinguishes cohort label/range, China-specific/general notes, permanent childlessness/fertility rate, and dataset/cohort year.
- 1: Mentions one distinction but leaves definitions partly unclear.
- 0: Conflates cohort and dataset years.

**Use of Evidence**
- 2: Uses official source note evidence and corroborates only compatible definition/context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated demographic data.

**Clarity and Structure**
- 2: Clear mapping table/list with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing cohort explanation.

### Common Failure Modes

- Treating 1935 or 1955 as single birth years.
- Swapping dataset years.
- Reporting fertility rates rather than childlessness estimates.
- Ignoring that the definitions are China-specific notes.

### Borderline Cases

- A table is acceptable and may improve clarity.
- Do not require explanation of childlessness methodology beyond the note boundaries.
- Partial credit if one dataset mapping is missing but cohort ranges are correct.

---

## 7. BND-CORE-PAIR-010

rubric_id: CORE-RUBRIC-B07-BND-CORE-PAIR-010
task_type: Core
research_object: cloud-accounting platform customer-acquisition cost
answer_unit: average cost per gross subscriber added and adjusted sales-marketing share

### Key Facts From Source Bundle

- Average cost of acquiring a subscriber increased to **$598 per gross subscriber added**.
- Adjusted sales and marketing costs would have been **31.2% of operating revenue**.
- The reported sales and marketing share was **32.5%**.
- The adjusted share is **1.3 percentage points lower** than reported.
- Gross subscriber added is distinct from net subscriber growth.
- Average acquisition cost is distinct from total sales spend.
- Percentage-point difference is distinct from percent difference.

### Expected Response Sections

- Conclusion with subscriber acquisition cost, adjusted share, reported share, and difference.
- Source comparison anchored in the official company report.
- Boundary explanation about gross/net subscribers, average/total costs, adjusted/reported percentages, and percentage points.
- Caveat about adjustment basis.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes $598, 31.2%, 32.5%, 1.3 pp, boundaries, evidence, caveat, and confidence.
- 1: Includes most figures but omits comparison or boundary.
- 0: Does not answer acquisition cost/share.

**Accuracy**
- 2: Reports **$598 per gross subscriber added**, **31.2%**, **32.5%**, and **1.3 percentage points lower**.
- 1: Gets most numeric facts but misses one component.
- 0: Reports net subscriber cost or treats 31.2% as total revenue.

**Reasoning**
- 2: Distinguishes gross/net subscriber, average/total spend, adjusted/reported percentage, and percentage-point/percent difference.
- 1: Mentions one boundary but leaves adjustment unclear.
- 0: Conflates cost, revenue, and marketing share.

**Use of Evidence**
- 2: Uses official company report and corroborates only compatible reporting/adjustment context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported SaaS benchmarks or unrelated company metrics.

**Clarity and Structure**
- 2: Clear multi-metric answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing customer-acquisition summary.

### Common Failure Modes

- Reporting net subscriber cost.
- Omitting the reported 32.5% comparison.
- Treating 31.2% as total operating revenue.
- Confusing percentage points and percent change.

### Borderline Cases

- Accept "$598 CAC" only if gross subscriber basis is clear.
- Do not require explaining the full adjustment calculation.
- If the 1.3 percentage-point difference is not stated but 31.2 and 32.5 are correct, accuracy is partial.

---

## 8. BND-CORE-PAIR-012

rubric_id: CORE-RUBRIC-B07-BND-CORE-PAIR-012
task_type: Core
research_object: AI automation labour-risk estimate
answer_unit: share of jobs in occupations at highest automation risk

### Key Facts From Source Bundle

- Occupations at highest risk of automation account for about **28% of jobs**.
- Highest-risk occupations are distinct from all AI-exposed jobs.
- Task substitution is distinct from actual job loss.
- Occupation share is distinct from an individual worker probability.
- Later estimates may account differently for complementarity.
- The estimate is methodology-sensitive.

### Expected Response Sections

- Conclusion with the about-28% job-share estimate.
- Source comparison anchored in the official analytical source.
- Boundary explanation about highest risk, exposure, task substitution, worker probability, and methodology.
- Caveat about complementarity and later estimates.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes 28%, highest-risk scope, method boundaries, evidence, caveat, and confidence.
- 1: Gives 28% but omits highest-risk or caveat boundaries.
- 0: Does not answer automation-risk share.

**Accuracy**
- 2: Reports about **28% of jobs** in occupations at highest automation risk.
- 1: Gives 28% but labels it imprecisely.
- 0: Says 28% of jobs will disappear or reports all AI exposure.

**Reasoning**
- 2: Distinguishes highest-risk/all exposed jobs, task substitution/job loss, occupation share/worker probability, and older/later methodologies.
- 1: Mentions one boundary but leaves risk interpretation unclear.
- 0: Treats occupation-level exposure as individual job-loss probability.

**Use of Evidence**
- 2: Uses official analytical source and corroborates only compatible methodology estimates.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic AI job-loss claims.

**Clarity and Structure**
- 2: Clear estimate with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Alarmist or unclear automation answer.

### Common Failure Modes

- Saying 28% of jobs will disappear.
- Reporting all AI exposure instead of highest automation risk.
- Treating occupation-level share as individual risk.
- Ignoring methodology differences across studies.

### Borderline Cases

- Accept "roughly 28%" or "about 28%."
- If another estimate is cited, it must be compared methodologically rather than replacing the source answer.
- Do not require occupation list retrieval.

---

## 9. BND-CORE-PAIR-020

rubric_id: CORE-RUBRIC-B07-BND-CORE-PAIR-020
task_type: Core
research_object: Japan gender employment gap context in 2024 labour note
answer_unit: gender employment gap and unpaid-care context

### Key Facts From Source Bundle

- Japan's gender employment gap is **21.3%**.
- It is the fourth highest among the relevant peer countries.
- Time spent on unpaid care and domestic work is also among the highest.
- Employment gap is distinct from wage gap.
- Ranking position is distinct from absolute value.
- Unpaid-care time is distinct from paid employment.
- The comparison is cross-country, not domestic-only.

### Expected Response Sections

- Conclusion with the employment gap, ranking, and unpaid-care context.
- Source comparison anchored in the official labour-market note.
- Boundary explanation about employment/wage gap, ranking/value, unpaid/paid work, and benchmark group.
- Caveat about comparison group and measurement scope.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes gap, ranking, unpaid-care context, evidence, caveat, and confidence.
- 1: Gives the gap but omits ranking or unpaid-care context.
- 0: Does not answer Japan gender employment gap context.

**Accuracy**
- 2: Reports **21.3%**, fourth highest, and unpaid care/domestic work among the highest.
- 1: Gets gap and one context element correct.
- 0: Reports gender wage gap or treats fourth highest as the value.

**Reasoning**
- 2: Distinguishes employment/wage gap, ranking/value, unpaid/paid work, and cross-country/domestic comparison.
- 1: Mentions one distinction but leaves comparison scope unclear.
- 0: Applies 21.3% to all gender labour gaps.

**Use of Evidence**
- 2: Uses official labour-market note and corroborates only compatible gender/labour indicators.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated gender wage statistics.

**Clarity and Structure**
- 2: Clear gap-plus-context answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing gender-labour answer.

### Common Failure Modes

- Reporting gender wage gap.
- Omitting the unpaid-care context.
- Treating fourth highest as the value.
- Applying the 21.3% figure to all labour-market gaps.

### Borderline Cases

- If the answer says "employment rate gap" instead of "employment gap," accept if meaning is clear.
- Do not require exact unpaid-care hours if the source only gives ranking context.
- Peer-country group should be caveated if not named.

---

## 10. CORE-GEN-05

rubric_id: CORE-RUBRIC-B07-CORE-GEN-05
task_type: Core
research_object: public-service satisfaction in trust survey
answer_unit: share of recent users satisfied with national health services

### Key Facts From Source Bundle

- **52%** of recent users of national health services reported relative satisfaction.
- The population is recent users, not the whole population.
- The service is national health services, not all public services.
- Satisfaction is distinct from trust in government.
- Survey wave and later releases may affect comparisons.
- "Relative satisfaction" should be preserved if the source uses that wording.

### Expected Response Sections

- Conclusion with the 52% share and respondent scope.
- Source comparison anchored in the official trust survey.
- Boundary explanation about recent users, service category, satisfaction, and trust.
- Caveat about survey wave and later releases.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes 52%, recent-user scope, service category, evidence, caveat, and confidence.
- 1: Gives 52% but omits scope or caveat.
- 0: Does not answer health-service satisfaction.

**Accuracy**
- 2: Reports **52%** of recent users satisfied with national health services.
- 1: Gives 52% with unclear respondent/service scope.
- 0: Applies 52% to whole population, all services, or political trust.

**Reasoning**
- 2: Distinguishes recent users/whole population, national health services/all services, satisfaction/trust, and survey wave/later releases.
- 1: Mentions one boundary but leaves scope unclear.
- 0: Confuses service satisfaction with government trust.

**Use of Evidence**
- 2: Uses official survey source and corroborates only compatible survey context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated public-opinion data.

**Clarity and Structure**
- 2: Clear survey-share answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Broad trust/public-services answer.

### Common Failure Modes

- Reporting whole-population satisfaction.
- Confusing public-service satisfaction with political trust.
- Applying 52% to all public services.
- Omitting recent-user scope.

### Borderline Cases

- "A majority, 52%" is acceptable.
- Do not require country-specific breakdowns if not in the answer unit.
- Later survey waves should be caveated, not silently substituted.

---

## 11. CORE-POL-18

rubric_id: CORE-RUBRIC-B07-CORE-POL-18
task_type: Core
research_object: Netherlands open-data legal update and reuse monitoring
answer_unit: June 2024 legal implementation and portal reuse-monitoring methods

### Key Facts From Source Bundle

- A public-sector information reuse act was adopted in **June 2024**.
- It fully implements the relevant public-sector open-data directive.
- The national data portal analyses usage metrics.
- The portal conducts user interviews.
- The statistical office hosts user days.
- Legal implementation is distinct from portal functionality.
- Usage metrics, interviews, and user days are different reuse-support/monitoring mechanisms.
- The answer should use Netherlands-specific factsheet content.

### Expected Response Sections

- Conclusion with June 2024 legal implementation and reuse-monitoring methods.
- Source comparison anchored in the official Netherlands factsheet.
- Boundary explanation about legal implementation versus portal methods and metric/interview/user-day distinctions.
- Caveat about country-specific 2024 factsheet status and later updates.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes legal update, directive implementation, all three monitoring/support methods, evidence, caveat, and confidence.
- 1: Includes legal update and some methods but omits one method or caveat.
- 0: Does not answer legal update and monitoring methods.

**Accuracy**
- 2: Reports **June 2024** act/directive implementation plus usage metrics, user interviews, and user days.
- 1: Gets legal update and at least two methods correct.
- 0: Omits June 2024 update or uses another country's factsheet.

**Reasoning**
- 2: Distinguishes legal implementation/portal functionality, usage metrics/interviews/user days, continuous analytics/user events, and Netherlands/nearby records.
- 1: Mentions one boundary but leaves method roles unclear.
- 0: Treats legal implementation as dataset availability or user days as the only monitoring method.

**Use of Evidence**
- 2: Uses Netherlands-specific official factsheet evidence and corroborates only compatible legal/portal context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses neighbouring country records or generic portal methods.

**Clarity and Structure**
- 2: Clear legal-plus-methods answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing open-data maturity answer.

### Common Failure Modes

- Omitting the June 2024 legal update.
- Treating user days as the only reuse-monitoring method.
- Confusing implementation of law with dataset availability.
- Mixing in another country's portal methods.

### Borderline Cases

- Accept "PSI reuse act" if it clearly refers to the public-sector information reuse act.
- User days may be framed as reuse engagement/support rather than continuous monitoring if metrics/interviews are separately identified.
- Later legal updates should be caveated separately.

---

## 12. CORE-POL-17

rubric_id: CORE-RUBRIC-B07-CORE-POL-17
task_type: Core
research_object: Luxembourg parliamentary open-data reuse support
answer_unit: mechanisms used to support creative data reuse and media needs

### Key Facts From Source Bundle

- The Parliament publishes relevant datasets.
- It incorporates journalist feedback.
- It organises hackathons.
- These actions support creative data reuse.
- They are intended to meet media needs.
- Parliamentary actions are distinct from whole-government open-data policy or national portal maturity scores.
- Journalist feedback is distinct from general user feedback.
- Hackathons are distinct from regular publication.

### Expected Response Sections

- Conclusion with the mechanisms and purpose.
- Source comparison anchored in the official Luxembourg factsheet.
- Boundary explanation about parliamentary versus national actions, journalist/media focus, and hackathons/publication.
- Caveat about audience/scope and reuse evidence.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes datasets, journalist feedback, hackathons, creative reuse/media purpose, evidence, caveat, and confidence.
- 1: Includes two mechanisms but omits purpose or caveat.
- 0: Does not answer reuse-support mechanisms.

**Accuracy**
- 2: Correctly states publishing datasets, incorporating journalist feedback, and organising hackathons for creative reuse/media needs.
- 1: Gets two mechanisms correct.
- 0: Reports only national maturity scores or generic portal support.

**Reasoning**
- 2: Distinguishes parliamentary/national policy, journalist/general feedback, hackathons/publication, and media/all reuse audiences.
- 1: Mentions one boundary but leaves audience/scope unclear.
- 0: Treats hackathons as continuous monitoring or whole-government policy.

**Use of Evidence**
- 2: Uses Luxembourg-specific official factsheet evidence and corroborates only compatible parliamentary context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses generic open-data engagement claims.

**Clarity and Structure**
- 2: Clear mechanism-purpose answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Broad open-data support answer.

### Common Failure Modes

- Reporting only dataset publication.
- Treating hackathons as continuous monitoring.
- Confusing parliamentary support with whole-government open-data policy.
- Omitting the media/journalist angle.

### Borderline Cases

- If "media users" replaces "journalists", accept when the journalist feedback mechanism remains clear.
- Do not require quantitative impact evidence.
- Parliamentary scope must remain explicit for full reasoning credit.

---

## 13. CORE-SCI-13

rubric_id: CORE-RUBRIC-B07-CORE-SCI-13
task_type: Core
research_object: Indonesia early-childhood centre principal survey
answer_unit: survey timing, population, and collection channel

### Key Facts From Source Bundle

- Data were collected in **March 2022**.
- Collection used an **electronic quantitative survey**.
- The survey was made available through the education-data management platform.
- The target population was all registered early-childhood centres.
- The centres served children from birth to age **6**.
- The respondent role concerns principals, not teachers or parents.
- Survey availability is distinct from completed response rate.

### Expected Response Sections

- Conclusion with timing, survey type/channel, target population, age coverage, and respondent role.
- Source comparison anchored in the primary study source.
- Boundary explanation about registered/all centres, principals/other respondents, age coverage, and availability/response.
- Caveat about response/completion status.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes timing, electronic survey, platform, registered centres, birth-age-6 coverage, respondent role, evidence, caveat, and confidence.
- 1: Includes timing and channel but omits population or respondent boundary.
- 0: Does not answer survey timing/population/channel.

**Accuracy**
- 2: Reports **March 2022**, electronic quantitative survey via education-data management platform to registered early-childhood centres serving birth to age 6.
- 1: Gets timing/channel but incomplete population detail.
- 0: Gives wrong year or describes child assessment data instead.

**Reasoning**
- 2: Distinguishes registered/all centres, principals/teachers/parents, birth-to-age-6/compulsory-school age, and availability/response rate.
- 1: Mentions one boundary but leaves survey population unclear.
- 0: Treats all centres as respondents or confuses survey type.

**Use of Evidence**
- 2: Uses the primary study source and corroborates only compatible methodology details.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated education statistics or programme descriptions.

**Clarity and Structure**
- 2: Clear methodology answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing survey-method answer.

### Common Failure Modes

- Reporting a different survey year.
- Treating all early-childhood centres as respondents.
- Omitting the electronic/platform collection channel.
- Confusing principal survey with child assessment data.

### Borderline Cases

- If "online survey" is used, accept if electronic/platform channel is clear.
- Do not require exact response rate.
- "Early childhood education centres" is acceptable if registered-centre scope is preserved.

---

## 14. CORE-TECH-01

rubric_id: CORE-RUBRIC-B07-CORE-TECH-01
task_type: Core
research_object: African national cybersecurity institution coverage
answer_unit: number of surveyed countries with national CERTs and national cybersecurity strategies

### Key Facts From Source Bundle

- The denominator is **44 surveyed African countries**.
- **13** surveyed countries had a national CERT.
- **14** surveyed countries had a national cybersecurity strategy.
- The region was characterised as the weakest global performer on both indicators.
- Surveyed countries are distinct from all African countries.
- National CERT is distinct from broader incident-response capacity.
- Cybersecurity strategy is distinct from cybersecurity law.
- Regional-performance claim is distinct from individual-country status.

### Expected Response Sections

- Conclusion with denominator, both counts, and regional-performance note.
- Source comparison anchored in the official digital-governance source.
- Boundary explanation about surveyed denominator, CERT/strategy definitions, and regional/individual status.
- Caveat about survey coverage and update status.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes denominator, CERT count, strategy count, performance note, evidence, caveat, and confidence.
- 1: Includes counts but omits denominator or performance note.
- 0: Does not answer cybersecurity institution coverage.

**Accuracy**
- 2: Reports **13 national CERTs** and **14 national cybersecurity strategies** out of **44 surveyed countries**, weakest performer on both.
- 1: Gets counts but omits denominator or swaps context.
- 0: Swaps counts, uses all African countries denominator, or reports laws as strategies.

**Reasoning**
- 2: Distinguishes surveyed/all countries, national CERT/incident response capacity, strategy/law, and regional/individual claims.
- 1: Mentions one boundary but leaves definitions unclear.
- 0: Conflates laws, strategies, CERTs, and general capacity.

**Use of Evidence**
- 2: Uses official digital-governance evidence and corroborates only compatible survey/update details.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unsupported cybersecurity rankings.

**Clarity and Structure**
- 2: Clear count/denominator answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing cybersecurity capacity answer.

### Common Failure Modes

- Using all African countries as denominator.
- Swapping the CERT and strategy counts.
- Treating cybersecurity laws as strategies.
- Omitting the 44-country surveyed denominator.

### Borderline Cases

- "Computer emergency response team" is acceptable for CERT.
- Do not require listing the 44 countries.
- Regional-performance note can be concise.

---

## 15. BND-CORE-PAIR-025

rubric_id: CORE-RUBRIC-B07-BND-CORE-PAIR-025
task_type: Core
research_object: private infrastructure investment market composition in 2023
answer_unit: primary-market growth and low- and middle-income country share in secondary markets

### Key Facts From Source Bundle

- Private investment in infrastructure projects in primary markets increased by **10% in nominal terms in 2023**.
- Low- and middle-income countries represented around **12%** of global secondary-market volumes.
- Primary markets are distinct from secondary markets.
- Nominal growth is distinct from real growth.
- LMIC share is distinct from developed-market contribution.
- 2023 observed data are distinct from preliminary 2024 rebound signals.

### Expected Response Sections

- Conclusion with 10% primary-market growth and 12% LMIC secondary-market share.
- Source comparison anchored in the official market report.
- Boundary explanation about primary/secondary markets, nominal/real growth, LMIC/developed contribution, and 2023/2024 timing.
- Caveat about market definitions and preliminary later signals.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes both figures, market boundaries, timing, evidence, caveat, and confidence.
- 1: Gives both figures but omits market or timing boundary.
- 0: Omits one of the two answer components.

**Accuracy**
- 2: Reports **10% nominal primary-market growth in 2023** and **around 12% LMIC share of secondary-market volumes**.
- 1: Gets both values but labels one market imprecisely.
- 0: Applies 10% to secondary markets or 12% to primary markets.

**Reasoning**
- 2: Distinguishes primary/secondary markets, nominal/real growth, LMIC/developed-market share, and 2023/preliminary 2024 data.
- 1: Mentions one distinction but leaves market composition unclear.
- 0: Mixes market layers or timing.

**Use of Evidence**
- 2: Uses official market-report evidence and corroborates only compatible market-definition/update context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses unrelated infrastructure investment figures.

**Clarity and Structure**
- 2: Clear two-part market answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing infrastructure-finance answer.

### Common Failure Modes

- Applying the 10% growth to secondary markets.
- Treating 12% as primary-market share.
- Reporting real growth without evidence.
- Mixing 2024 preliminary signals into the 2023 answer.

### Borderline Cases

- Accept "about 12%" for around 12%.
- If 2024 rebound is mentioned, it must be separated from the 2023 answer.
- Do not require absolute investment volumes.

---

## 16. BND-CORE-PAIR-028

rubric_id: CORE-RUBRIC-B07-BND-CORE-PAIR-028
task_type: Core
research_object: regional open-data policy maturity dimension in 2024
answer_unit: average policy-dimension maturity level and change since 2023

### Key Facts From Source Bundle

- Policy has been the most mature open-data dimension on average since **2015**.
- The 2024 policy-dimension average is **91%**.
- The change since 2023 is a **2 percentage-point increase**.
- Policy dimension is distinct from overall maturity score.
- Percentage-point change is distinct from percent change.
- Regional average is distinct from individual-country results.
- Long-running dimension rank is distinct from a single-year score.

### Expected Response Sections

- Conclusion with 2024 average, change since 2023, and since-2015 rank context.
- Source comparison anchored in the official maturity report.
- Boundary explanation about policy dimension, overall maturity, percentage points, and regional average.
- Caveat about report-year and methodology revisions.
- Confidence level.

### Fixed Criteria, 0-2 Each

**Coverage**
- 2: Includes 91%, 2 percentage-point increase, since-2015 context, evidence, caveat, and confidence.
- 1: Gives 91% and change but omits rank context or caveat.
- 0: Does not answer policy-dimension maturity.

**Accuracy**
- 2: Reports **91%** in 2024, **2 percentage-point** increase since 2023, and most mature since **2015**.
- 1: Gets two of the three components correct.
- 0: Reports overall maturity or treats 2 percentage points as 2%.

**Reasoning**
- 2: Distinguishes policy dimension/overall score, percentage-point/percent change, regional/individual country results, and long-running rank/single-year score.
- 1: Mentions one boundary but leaves score meaning unclear.
- 0: Applies regional average to every country or wrong dimension.

**Use of Evidence**
- 2: Uses official maturity report evidence and corroborates only compatible methodology/year context.
- 1: Uses one relevant source with limited comparison.
- 0: Uses country factsheets or portal summaries as the policy-dimension average without support.

**Clarity and Structure**
- 2: Clear maturity-dimension answer with caveat and confidence.
- 1: Mostly clear but incomplete.
- 0: Confusing open-data maturity answer.

### Common Failure Modes

- Reporting overall maturity instead of policy-dimension maturity.
- Treating 2 percentage points as 2%.
- Applying the regional average to every country.
- Omitting the since-2015 maturity-rank context.

### Borderline Cases

- "Two-point increase" is acceptable if clearly percentage points.
- Do not require country-level examples.
- Later methodology revisions should be caveated separately.
