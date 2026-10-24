# Central Asian herbarium digitization

Supporting data and code for **Awakening dormant historical plant specimens of Central Asia: from complex labels to reusable biodiversity information**, manuscript P16.

## Contents

| Directory inside the package | Research materials |
| --- | --- |
| `baseline_P12/` | Saved recognition and extraction outputs, reference retrieval, anonymous human reviews and adjudications, paired geographic records, resource curation, configurations, code and figure source data |
| `update_P15/derived/` | Current P16 specimen and spatial records: 319 specimens, 269 with spatial results (84.33%), and 148 with both scientific-name readings and spatial information |
| `update_P15/quality_audit/` | Frozen 60-specimen sample, review decisions, weighted estimates before corrections, statistical method and correction records |
| `update_P15/historical49/` | Historical cohort use, split roster and saved rechecks supporting Supplementary Table S24 |
| `update_P15/code/` | Existing quality-analysis and correction scripts, with their input and layout documentation |
| `figures_P16/` | Current English Figures 1, 3, 4 and 5 in editable SVG and PDF |
| `docs/` | Evidence map connecting main Tables 1–5 and Supplementary Tables S1–S24 to the released files |

The versioned directories distinguish the earlier records from the reviewed record state used in P16. The 60-specimen quality estimates describe records before the recorded corrections. The current derived records and those pre-correction estimates retain their respective time points.

## Review and execution provenance

Human verification of the historical AI-assisted working suggestions, all stages of the 50/15-specimen review, the 60-specimen quality review and the geographic interpretations was confirmed by the author on 25 October 2026. Original outputs, unresolved cases and quantitative review denominators remain unchanged. The interactive geographic-session model is identified by the author as GPT 6 Astra; archived Gemini API records and Claude/DeepSeek extraction records retain their recorded model identifiers. Model-identification provenance is stored with the affected records. Final human checking is now explicitly synchronized across the current specimen CSV/JSONL and spatial JSONL, including the nine administrative subrecords. All 60 final place-name-link dispositions were individually checked and confirmed by humans, including retained unresolved outcomes. Original generation-stage flags remain explicitly historical; see `baseline_P12/docs/DATA_DICTIONARY.md` inside the ZIP. No new independent reviewer or quality observations are claimed.

## Use and source access

Extract the package before use. Files ending in `.jsonl.gz` contain gzip-compressed UTF-8 JSON Lines. From the extracted `baseline_P12` directory, `python code/export_tables.py` exports descriptive tables from saved baseline results. The quality-analysis scripts in `update_P15/code/` retain the original project-layout assumptions documented in their README.

Image-level reproduction additionally requires the original specimen images/crops, annotations, fine-tuned model weights, catalogue and reference databases, and the relevant configuration. These complete external inputs are not included. Figure 2 contains specimen photographs and is not distributed in this package. Provider URLs, versions and source-specific access terms are recorded in the source register; those terms continue to apply.

`project/`, `external_dataset/`, `external_specimen_images/`, `external_local/` and `skill/` identify upstream source locations requiring local configuration. Embedded historical hashes identify original source artifacts. `SOURCE_FILES.csv` maps copied files to their upstream and released hashes, and `SHA256SUMS.txt` records the actual package contents.

Supplementary Table S1 is supported by both the saved validation summary and the existing development-set summary (`paddle_fixed_update_dev49_summary.csv`, `fixed_final180` rows); the development report was added without rerunning an experiment.

## Download and file index

- [P16 supporting data and code](./reproducibility_revision16.zip) — 224 files; 4,919,355 bytes.
- [Evidence map](./EVIDENCE_MAP.md)
- [Source access and terms](./SOURCE_ACCESS.csv)
- [Package file list and checksums](./PACKAGE_CONTENTS.csv)
- [ZIP SHA-256](./PACKAGE_SHA256.txt)

## Access to complete original inputs for review

On request, the authors can provide editors and reviewers with original files or access links for the complete original specimen images and crops, annotations, regional catalogue workbook, reference and geographic databases, and fine-tuned model weights. This review-access arrangement does not mean that all of these inputs are included in this public download; provider-specific terms continue to apply.
