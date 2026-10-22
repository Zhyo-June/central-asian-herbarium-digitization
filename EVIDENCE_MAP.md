# Evidence map

| Article evidence | Released files |
| --- | --- |
| Table 1 / Figure 4 resource counts | `sources/build_manifest.json`, `tables/rag_database_inventory.json`, `tables/catalogue_family_counts.csv` |
| Table 2 / Figure 3b and Supplementary Table S5 | `tables/per_field_counts.csv`, `tables/unified319_summary.json`, `outputs/selected_outputs.jsonl.gz`, `outputs/catalogue_references.json` |
| Table 3 / Figure 3c / Supplementary Tables S7–S9 | `human/human_method_ratings.csv`, `human/human_candidate_ratings.csv`, `human/all50_by_readability.csv`, `human/partial_locality_cases.csv` |
| Reviewer agreement | `human/agreement.json`, `human/reviewer_disagreements.csv` |
| Supplementary Table S1 | `tables/detector_fixed20_all_runs.csv` |
| Supplementary Table S2 attribution and protocol | `config/paddle_fixed_update_protocol.json`, `config/paddle_fixed_update_runtime.json` |
| Figure 3a line recognition | `tables/manual_line_figure_values.csv` |
| Supplementary Table S3 / Figure 4c | `retrieval/benchmark_queries.jsonl`, `retrieval/query_outcomes.csv`, `retrieval/metrics.json`, `retrieval/ranked_results.jsonl.gz` |
| Supplementary Table S4 thresholds | `tables/metrics_side_by_side.csv`, `tables/unified319_summary.json` |
| Supplementary Table S6 model composition | `tables/selected_model_counts.csv`, `outputs/selected_outputs.jsonl.gz` |
| Supplementary Table S10 directed review | `human/rag_human_case_results.csv` |
| Supplementary Table S11 costs | `tables/cost_summary.json`, `outputs/request_metadata.jsonl.gz` |

The public package supports examination of saved outputs and regeneration of reported descriptive tables. Image-based rescoring additionally needs the original crops and annotated lines. Rebuilding the 86,705-record resource additionally needs the original workbook and source databases. Fine-tuned weights, full scans and the complete catalogue workbook are not included in this release.
