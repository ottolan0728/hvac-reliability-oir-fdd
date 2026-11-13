# OIR-FDD: Cross-System HVAC Fault Diagnosis Reliability

Companion repository for the submission-stage manuscript:

*When Cross-System HVAC Fault Diagnosis Fails: Source-Class Discrimination, Fault Retention, and Sensor Availability*

Authors: Chun-Jan Tseng, Yi-Kai Su, and Ming-Han Chang.

## Scope

The Observability–Identifiability–Reliability framework (OIR-FDD) organizes physical eligibility, Identifiability-Gated Transfer Interpretation (IGTI), and Class-Retention Reliability Audit (CRRA). These are deterministic post-evaluation evidence audits, not newly trained fault classifiers. Two complementary equipment experiments are deliberately not treated as independent replications.

## Public evidence release

The `derived_results/` directory contains eight non-restricted frozen aggregate tables corresponding to Supplementary Tables S1–S8:

- `S1_RTU_baseline_summary.csv`
- `S2_fault_support.csv`
- `S3_calibration_support.csv`
- `S4_equal_coverage_summary.csv`
- `S5_fallback_recovery_RTU.csv`
- `S6_class_interpretation_evidence.csv`
- `S7_pairwise_separability.csv`
- `S8_ablation_summary.csv`

These tables are presentation extracts from frozen experimental results; they do not constitute independent raw observations or new model runs.

## Repository structure and limitations

- `algorithms/`: deterministic conceptual specifications; not executable implementations.
- `data_manifest/`: initial provenance notes, not a complete machine-checkable split manifest.
- `derived_results/`: non-restricted aggregate tables for inspecting reported evidence.
- `manuscript/` and `supplementary/`: historical LaTeX source snapshots, **not** the authoritative current R54 submission package.
- `reproducibility/`: methodological boundaries and evidence rules.

The original HVAC datasets must be obtained from their providers under applicable terms; no third-party raw dataset is redistributed here. The repository does **not** currently supply an end-to-end executable model-training reproduction, full environment lockfiles, or a verified complete split/eligibility manifest. Claims of complete computational reproducibility would therefore be inappropriate. The frozen manuscript submission and its supplementary PDF remain the authoritative reporting artifacts.

## Citation

See `CITATION.cff`; the final bibliographic record should be updated after publication.
