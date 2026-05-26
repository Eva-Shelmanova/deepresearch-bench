# DeepResearch Benchmark Final Package

This repository now contains the final benchmark package built from the Core and Set source extraction workflow through manual prompt/rubric construction.

## Main File

- `final.xlsx` - final two-sheet benchmark table:
  - `Core`: Core tasks with English and Russian prompt/rubric columns.
  - `Set`: Set tasks with English and Russian prompt/gold-set columns.

## Source Artifacts

- `manual_prompt_rewrite_batch_001.md`
- `manual_deep_research_batch_002.md` through `manual_deep_research_batch_012.md`
- `batch_1_rubrics.md` through `batch_12_rubrics.md`
- `Benchmark Plan.pdf`

Large raw source folders, text-extraction outputs, exploratory scripts, logs, and intermediate spreadsheets are excluded from git. They were kept locally in an archive during cleanup rather than committed.
# DeepResearch Bench Source Pipeline

This repository contains a lightweight, readable extraction and clustering pipeline for building Core-style benchmark source packets from a local folder of benchmark documents.

Raw source files are intentionally **not included** in this repository. The local `core/`, `raw_text/`, and Python virtual environment folders are excluded because they are large and/or derived artifacts.

For a full description of what was built, how each script works, and what the outputs mean, see **[PIPELINE_OVERVIEW.md](PIPELINE_OVERVIEW.md)**.

## Included Artifacts

- `raw_sources_index.csv` - source-file index with extraction status, hashes, duplicate indicators, and output paths.
- `core_extraction.xlsx` - quality-gated source packet with canonical IDs, excerpts, domains, comparison dimensions, synthesis potential, QA levels, and final decisions.
- `core_clusters.xlsx` - 2-3 source clusters built only from `COMPLETE` rows, plus summary and cluster QA sheets.
- `core_prompt_drafts.xlsx` - 73 draft synthesis prompts, one per ready cluster; includes source excerpt previews, axis-debug, and QA sheets.
- `core_rubrics.xlsx` - Phase X evaluation artifacts: 365 axis-anchored rubric rows (73 clusters × 5 criteria), source excerpts for key-fact extraction, and a summary sheet.
- `core_model_pilot_inputs.jsonl` / `core_model_pilot_inputs.xlsx` - model-ready Core task packets for Phase XII pilot runs.
- `CORE_PRE_API_READINESS.md` - final pre-API status report with translation, rubric, and pilot-input counts.
- `core_extraction_manual_audit.md` - audit notes from the source-packet QA pass.

## Pipeline Scripts

Run from the repository root:

```bash
python3 -m venv .venv
.venv/bin/pip install -r requirements.txt
```

Then, with a local `core/` folder available:

```bash
.venv/bin/python extract_raw_sources.py
.venv/bin/python select_core_excerpts.py
.venv/bin/python build_core_source_packet.py
.venv/bin/python build_core_clusters.py
.venv/bin/python add_cluster_qa.py
.venv/bin/python remediate_needs_review_clusters.py
.venv/bin/python build_core_prompt_drafts.py
.venv/bin/python build_core_rubrics.py
.venv/bin/python prepare_core_pre_api_package.py --translate-non-english
```

When ready to make the first real model API calls, run the optional OpenAI-compatible pilot runner:

```bash
OPENAI_API_KEY=... OPENAI_MODEL=gpt-4o-mini \
  .venv/bin/python run_core_model_pilot_openai.py --limit 5
```

## Current Output Summary

- `core_extraction.xlsx`: 263 source rows, with 212 `COMPLETE` sources after duplicate and quality filtering.
- `core_clusters.xlsx`: 73 ready clusters using 212 complete sources; cluster sizes are 2-3 sources.
- `core_prompt_drafts.xlsx`: 73 draft Core synthesis prompts, one per ready cluster.
- `core_rubrics.xlsx`: 73 × 5 = 365 rubric rows with axis-anchored 0–2 descriptors, examples, failure modes, borderline notes, and pre-review key facts.
- `core_model_pilot_inputs.jsonl` / `core_model_pilot_inputs.xlsx`: 73 model-ready Core tasks with prompts, translated/source excerpts, and rubrics.

## Notes

- No LLM summarization is used for extraction or rubric generation.
- Duplicate variants are excluded from `COMPLETE` clustering.
- Translation preparation is complete for Core: 211 sources are English/no-translation-needed and 1 Dutch source has a curated English fallback translation.
- Raw source files must be supplied locally and are not committed to GitHub.
- Rubric `key_facts` and `expected_response_sections` are pre-review drafts. Human annotators should verify them in Phase XI before freezing results.

