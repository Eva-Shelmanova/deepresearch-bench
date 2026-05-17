# DeepResearch Bench Source Pipeline

This repository contains a lightweight, readable extraction and clustering pipeline for building Core-style benchmark source packets from a local folder of benchmark documents.

Raw source files are intentionally **not included** in this repository. The local `core/`, `raw_text/`, and Python virtual environment folders are excluded because they are large and/or derived artifacts.

## Included Artifacts

- `raw_sources_index.csv` - source-file index with extraction status, hashes, duplicate indicators, and output paths.
- `core_extraction.xlsx` - quality-gated source packet with canonical IDs, excerpts, domains, comparison dimensions, synthesis potential, QA levels, and final decisions.
- `core_clusters.xlsx` - 2-3 source clusters built only from `COMPLETE` rows, plus summary and cluster QA sheets.
- `core_prompt_drafts.xlsx` - draft synthesis prompts for ready clusters. Rubrics and model answers are not generated yet.
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
```

## Current Output Summary

- `core_extraction.xlsx`: 263 source rows, with 212 `COMPLETE` sources after duplicate and quality filtering.
- `core_clusters.xlsx`: 73 ready clusters using 212 complete sources; cluster sizes are 2-3 sources.
- `core_prompt_drafts.xlsx`: 73 draft Core synthesis prompts, one per ready cluster.

## Notes

- No LLM summarization is used for extraction.
- Duplicate variants are excluded from `COMPLETE` clustering.
- Translation is not yet complete; translation fields are marked as pending where applicable.
- Raw source files must be supplied locally and are not committed to GitHub.

