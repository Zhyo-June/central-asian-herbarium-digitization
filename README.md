# Central Asian herbarium digitization

Reproducibility materials for **Digitizing historical Central Asian herbarium labels with complementary recognition routes and multilingual reference data**, manuscript revision 11 (22 October 2026).

The study connects domain-adapted OCR, direct visual reading and multilingual reference retrieval to historical specimen labels. The release packages existing experiment records; it adds no model runs or new human judgments.

## Download the package

[Download the revision11 reproducibility package](./reproducibility_revision11.zip). The archive contains 97 files in the classified directories below. Extract the archive before running the scripts. [PACKAGE_CONTENTS.csv](./PACKAGE_CONTENTS.csv) lists every file and its SHA-256; [EVIDENCE_MAP.md](./EVIDENCE_MAP.md) maps results to files inside the archive.

## Read the evidence

| Directory | Contents |
| --- | --- |
| `config/` | Full prompts, request settings, frozen field/human protocols and Paddle training-size protocol |
| `outputs/` | 319 selected A–F outputs, OCR/input metadata, catalogue references and request metadata |
| `human/` | Original anonymized ratings, readability strata, 31 reviewer disagreements and partial-locality examples |
| `retrieval/` | All 178 benchmark queries, target definitions, ranked outputs and group outcomes |
| `tables/` | Field scores, detector trajectories, recognition and resource figure values, cost summaries |
| `sources/` | Source/version/rights register and existing resource-preservation records |
| `code/` | Archived extraction/retrieval code, frozen alignment and saved-result table exporter |
| `figures/` | Editable SVGs for Figures 1, 3 and 4; Figure 2 requires the original specimen images |
| `docs/` | Evidence map and data dictionary |

The main comparison includes all 319 specimens, with 314 nonempty collector references. Character coverage aligns reference text to actual outputs; same-field coverage confines the source to the corresponding field. Human grades retain complete and partial transcription separately. A partial locality can preserve a usable geographic description, as in TASH117037, while other partial grades contain toponym errors.

## Regenerate the tables

With Python 3.10 or later, run `python code/export_tables.py`. This reads saved results and writes CSV tables to `generated/`; it makes no network requests and performs no new inference or statistical tests. Optional figure regeneration uses `python code/export_figures.py` with the packages in `code/requirements_figures.txt`. Gzipped JSONL files contain one ordinary JSON object per line and can also be decompressed directly.

Archived experiment scripts preserve the original project-relative layout. They document the inference and retrieval implementations; rerunning those pipelines additionally requires specimen crops, model checkpoints, the original catalogue and source databases, plus an explicitly configured API endpoint and credentials. The frozen alignment file is byte-identical to the original. Publication-only path substitutions in other scripts are recorded in `sources/file_provenance.csv`.

## Source access and rights

`sources/source_license_register.csv` records provider URLs, versions and source-specific terms. Full third-party scans and databases are accessed from their providers. This release contains experiment outputs, short name-based retrieval records and provenance metadata. It does not grant a new license over third-party material; no repository-wide reuse license has been assigned.

The source register and evidence map identify materials available here and additional inputs needed for image-level replication. `SHA256SUMS.txt` fixes the released file contents.
