# Core Extraction Manual Audit

Generated after tightening `build_core_source_packet.py` and regenerating `core_extraction.xlsx`.

## Status Rule

Only these row-level `final_decision` values are used:

- `COMPLETE`
- `PARTIAL`
- `NEEDS_REVIEW`
- `REJECTED`

`COMPLETE` is reserved for canonical, non-duplicate rows with at least 500 words, no detected extraction errors, quantitative evidence, comparison potential, synthesis potential, specific annotation fields, and no front-loaded boilerplate or dominant noise.

`translation_status` is explicitly set to `pending` because no translation pass has been run. This keeps the bilingual layer visible without treating the blank `translated_excerpt` as a parser failure.

## Final Counts

- `COMPLETE`: 212
- `PARTIAL`: 1
- `NEEDS_REVIEW`: 16
- `REJECTED`: 34

## Stratified Audit Sample

### COMPLETE Sample

Reviewed sample:
`S001`, `S029`, `S052`, `S066`, `S077`, `S090`, `S104`, `S115`, `S127`, `S141`, `S154`, `S169`, `S180`, `S192`, `S204`, `S216`, `S228`, `S240`

Audit result:
These rows passed the automated Core gate after the stricter noise rules. They contain non-empty source text, sufficient length, quantitative or date-based evidence, and usable comparison/synthesis fields. They remain eligible for clustering, subject to later human review for content-specific suitability.

### PARTIAL Sample

Reviewed sample:
`S035`

Audit result:
`S035` is meaningful but short (`300-499` words). It should not move directly into prompt writing without expansion from the raw source.

### NEEDS_REVIEW Sample

Reviewed sample:
`S025`, `S026`, `S027`, `S028`, `S093`, `S100`, `S136`, `S137`, `S138`, `S147`

Audit result:
These were correctly demoted out of `COMPLETE`. Reasons include multi-file source identity review (`S025`), legislation navigation/cookie/resource boilerplate (`S026`, `S027`, `S028`), corporate risk/forward-looking boilerplate (`S093`, `S100`), and questionnaire/table-like open-data fragments with unclear comparison or synthesis potential (`S136`, `S137`, `S138`, `S147`).

### REJECTED Rows Audited

Reviewed rejected set:
`S002`, `S003`, `S004`, `S006`, `S007`, `S008`, `S010`, `S012`, `S015`, `S017`, `S019`, `S030`, `S033`, `S034`, `S037`, `S039`, `S042`, `S044`, `S046`, `S051`, `S057`, `S059`, `S065`, `S083`, `S084`, `S099`, `S189`, `S202`, `S221`, `S237`, `S241`, `S249`, `S252`, `S255`

Audit result:
The rejected rows are not eligible for Core prompt writing in the current packet. Most are duplicate variants linked to a canonical source. The rest are too short, extraction-error affected, boilerplate dominated, table-only/financial-statement fragments, or lack evidence/synthesis potential.

## Fixes Applied From Audit

- Added exact four-status final decisions.
- Added `translation_status = pending`.
- Added `extraction_status`.
- Added `table_noise_ratio` and `front_loaded_noise`.
- Forced Excel-safe string cells to prevent formula interpretation and `#NAME?`.
- Removed file-boundary headers from normal candidate selection.
- Penalized and demoted:
  - cookie/navigation/resource blocks,
  - table-of-contents fragments,
  - forward-looking and SEC risk disclaimer blocks,
  - dense table-only fragments,
  - duplicate variants,
  - rows with weak comparison/synthesis fields.

## Remaining Caveat

This is now a stricter extraction packet, not a bilingual final packet. The next phase should either fill `translated_excerpt` or keep `translation_status = pending` until the translation layer is deliberately run.
