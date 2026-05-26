# Manual Prompt Rewrite Batch 001

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

## 1. CORE-POL-01

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_renamed
research_object: Poland's new fiscal oversight body
answer_unit: planned operational start date

source_anchor:
- The source context says Poland's Fiscal Council is set to begin operations on 1 January 2026.

internal_source_boundary:
- source_name: internal fiscal-governance source bundle
- source_scope: row/paragraph about Poland's new Fiscal Council start date

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For Poland's new fiscal oversight body, resolve planned operational start date.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish legal establishment, appointment/setup milestones, budget-year applicability, and the date when the fiscal oversight body is expected to begin operations. Return: current legal/status conclusion, source comparison, caveat, and confidence.

---

## 2. CORE-TECH-05

task_type: open_web_multi_source_uncertainty_research
manual_status: ready_after_rewrite
research_object: enterprise software renewable-electricity disclosure link
answer_unit: whether the link is direct, indirect, or unsupported

source_anchor:
- The source context combines company-level sustainability disclosures with system-level renewable-electricity transition evidence.

internal_source_boundary:
- source_name: internal company-disclosure / energy-transition source bundle
- source_scope: passages about company energy or emissions disclosure and renewable-electricity transition evidence

final_prompt_text:
Use the official primary source as anchor and one corroborating source if available. For enterprise software renewable-electricity disclosure link, resolve whether the link is direct, indirect, or unsupported.

Use `source_scope` only to locate the relevant row, note, paragraph, or table; do not infer beyond it. Methodological trap: distinguish company-level electricity procurement or emissions disclosure from system-level renewable-electricity outcomes, and separate correlation from causal contribution. Return: concise conclusion, source comparison, caveat, and confidence.

---

## 3. SET-GEN-F04

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
