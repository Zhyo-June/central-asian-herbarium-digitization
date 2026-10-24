# Evidence map for manuscript P16

Paths below are relative to the extracted `reproducibility_revision16.zip`. The table numbers follow the P16 English manuscript and supplementary information.

| P16 evidence | Existing released records |
| --- | --- |
| Table 1; Figure 4a: reference-resource organization | `baseline_P12/sources/build_manifest.json`, `baseline_P12/tables/rag_database_inventory.json`, `baseline_P12/tables/catalogue_family_counts.csv` |
| Figure 3a: line recognition | `baseline_P12/tables/manual_line_figure_values.csv`; detector records in `baseline_P12/tables/detector_fixed20_all_runs.csv` and `detector_100_epoch_training.csv` |
| Table 2; Figure 3b: extraction for 319 specimens | `baseline_P12/tables/per_field_counts.csv`, `baseline_P12/tables/unified319_summary.json`, `baseline_P12/outputs/selected_outputs.jsonl.gz`, `baseline_P12/outputs/catalogue_references.json` |
| Table 3; Figure 3c: image review and adjudication | `baseline_P12/human/human_method_ratings.csv`, `human_candidate_ratings.csv`, `method_ratings_after_adjudication.csv`, `adjudication31.json` |
| Table 4: three spatial-record stages | `baseline_P12/geography/spatial_records_paired.jsonl`, `baseline_P12/geography/spatial_coverage_paired.csv`, `update_P15/quality_audit/curation_summary.json`, `update_P15/derived/spatial_records_reviewed319.jsonl` |
| Table 5: quality of records before the current corrections | `update_P15/quality_audit/weighted_quality_before_corrections.csv`, `statistical_method.json`, `field_judgments_before_corrections.csv` |
| Figure 5: current spatial display | `update_P15/derived/map_reviewed319.geojson`, `update_P15/derived/spatial_records_reviewed319.jsonl`, `update_P15/figure_source_data/figure5_spatial_points.csv`; saved artwork in `figures_P16/` |
| S1: fixed-update Paddle comparison | `baseline_P12/tables/paddle_fixed_update_summary.csv`, `baseline_P12/config/paddle_fixed_update_protocol.json`, `baseline_P12/config/paddle_fixed_update_runtime.json` |
| S2; Figure 4b: retrieval benchmark | `baseline_P12/retrieval/benchmark_queries.jsonl`, `query_outcomes.csv`, `metrics.json`, `ranked_results.jsonl.gz` |
| S3: locality thresholds | `baseline_P12/tables/metrics_side_by_side.csv`, `baseline_P12/tables/unified319_summary.json` |
| S4: within-field character coverage | `baseline_P12/tables/per_field_counts.csv`, `baseline_P12/tables/unified319_summary.json` |
| S5: selected model labels | `baseline_P12/tables/selected_model_counts.csv`, `baseline_P12/outputs/selected_outputs.jsonl.gz` |
| S6–S7: original human grades and readability | `baseline_P12/human/human_method_ratings.csv`, `human_readable_summary.csv`, `all50_by_readability.csv`; agreement in `agreement.json` and `reviewer_disagreements.csv` |
| S8: partially recovered localities | `baseline_P12/human/partial_locality_cases.csv`, `geographic_usability19.json` |
| S9: directed review of RAG changes | `baseline_P12/human/rag_human_case_results.csv` |
| S10: recorded usage | `baseline_P12/tables/cost_summary.json`, `baseline_P12/outputs/request_metadata.jsonl.gz` |
| S11: original grades and adjudication | `baseline_P12/human/method_ratings_after_adjudication.csv`, `adjudication31.json`, `collector_amendment_sensitivity.csv`; `baseline_P12/tables/adjudication_sensitivity.csv` |
| S12: frozen paired geography | `baseline_P12/geography/spatial_summary.json`, `spatial_records_paired.jsonl`, `coordinates_paired.csv` |
| S13: initial resource review | `baseline_P12/human/resource_review271.json`, `baseline_P12/resource_curation/review_summary.json`, `baseline_P12/tables/resource_review_by_type.csv` |
| S14: 60 place-name link dispositions | `baseline_P12/resource_curation/links60_before_after.json`, `manual_review_applied.json`, `merged_issues.json` |
| S15–S16: reference and geographic modules | `baseline_P12/config/`, `baseline_P12/code/`, `baseline_P12/skill/`, `baseline_P12/resource_curation/`, `baseline_P12/sources/source_license_register.csv`; access limits in `README.md` |
| S17: linked information before/after review | `update_P15/baseline/joint_information_summary_revision14.json`, `update_P15/derived/joint_information_summary_revision15.json`, `update_P15/derived/specimen_information_records_reviewed319.jsonl` |
| S18: linkage in the existing 50-specimen review | Join specimen IDs in `baseline_P12/human/method_ratings_after_adjudication.csv` with `baseline_P12/geography/spatial_records_paired.jsonl`; original review scope is retained |
| S19: TASH070079 example | TASH070079 records in `update_P15/derived/specimen_information_records_reviewed319.jsonl`, `update_P15/derived/spatial_records_reviewed319.jsonl` and the frozen paired geography |
| S20: stratified sampling | `update_P15/quality_audit/sampling_plan.json`, `frozen_sample60.json`, `spatial_strata_before_corrections.json` |
| S21: original 60-specimen decisions | `update_P15/quality_audit/60份最终记录_质量核查_20261024015135.json`, `field_judgments_before_corrections.csv`, `review_import.json` |
| S22: complete weighted estimates | `update_P15/quality_audit/weighted_quality_before_corrections.csv`, `weighted_quality_before_corrections.json`, `statistical_method.json`; archived implementation in `update_P15/code/archived/analyse_review.py` |
| S23: implemented review changes | `update_P15/quality_audit/corrections_before_after.csv`, `corrections_before_after.json`, `review_dispositions60.json`, `supplemental_spatial_evidence.json`; archived implementation in `update_P15/code/archived/apply_review.py` |
| S24: historical 49-specimen use | `update_P15/historical49/historical49_timeline.json`, `historical49_roster_recheck.json`, `historical49_eligibility_updated.json`, `split_policy.json`, `splits.csv` and accompanying recheck records |

Where a row lists a directory once followed by bare filenames, all such filenames share that directory. Inspect recorded results directly; publishing this archive did not rerun these analyses. Raw images and fine-tuned model weights are not part of this archive. Figure 2 contains third-party specimen images and is not separately distributed here.
