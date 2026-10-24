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

## Methods and human review

AI was used for label interpretation and georeferencing, followed by human checking. The author confirmed completion of geographic checking and all 60 final place-name-link dispositions on 25 October 2026. The interactive geographic-session model is identified by the author as GPT 6 Astra; archived Gemini API records and Claude/DeepSeek extraction records retain their recorded model identifiers. Current records retain final human-review status, original human judgments, sources, unresolved evidence questions and the research results before and after correction. Record fields and version scopes are defined in baseline_P12/docs/DATA_DICTIONARY.md.

## Use and source access

Extract the package before use. Files ending in `.jsonl.gz` contain gzip-compressed UTF-8 JSON Lines. From the extracted `baseline_P12` directory, `python code/export_tables.py` exports descriptive tables from saved baseline results. The quality-analysis scripts in `update_P15/code/` retain the original project-layout assumptions documented in their README.

Image-level reproduction additionally requires the original specimen images/crops, annotations, fine-tuned model weights, catalogue and reference databases, and the relevant configuration. These complete external inputs are not included. Figure 2 contains specimen photographs and is not distributed in this package. Provider URLs, versions and source-specific access terms are recorded in the source register; those terms continue to apply.

`project/`, `external_dataset/`, `external_specimen_images/`, `external_local/` and `skill/` identify upstream source locations requiring local configuration. Embedded historical hashes identify original source artifacts. `SOURCE_FILES.csv` maps copied files to their upstream and released hashes, and `SHA256SUMS.txt` records the actual package contents.

## Download and file index

- [P16 supporting data and code](./reproducibility_revision16.zip) — 223 files; 4,896,723 bytes.
- [Evidence map](./EVIDENCE_MAP.md)
- [Source access and terms](./SOURCE_ACCESS.csv)
- [Package file list and checksums](./PACKAGE_CONTENTS.csv)
- [ZIP SHA-256](./PACKAGE_SHA256.txt)
