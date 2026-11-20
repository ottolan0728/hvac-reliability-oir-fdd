# HVAC sensor-loss decision reliability: companion evidence repository

Companion repository for the author-review manuscript:

**High-Confidence Fault Misses in HVAC Diagnosis Under Sensor Loss: A Source-Frozen Reliability and Decision Study**

Authors: Chun-Jan Tseng, Yi-Kai Su (corresponding author), and Ming-Han Chang. Intended journal: *IEEE Access*. **This is an unpublished submission-stage manuscript; no acceptance, DOI, or publication is claimed.**

## Current research question and evidence

The current paper examines how a source-frozen four-class HVAC diagnostic system changes its decisions when the reheat-valve-position input is persistently replaced by a source mean in transfer from simulated series to parallel fan-powered units. It traces the same target windows from correctly accepted fault decisions into accepted-normal, other-fault, or rejected states and evaluates a capacity-constrained review-priority rule.

In the shuffled-topology control, 42 initially correct, accepted valve-fault **model–seed decisions**, representing 35 distinct windows from one shared simulated setting, remain accepted but change to normal under the archived sensor-loss stress. These are **not** 42 independent fault events or 35 independent buildings. The low-normal-confidence review-priority heuristic is a **negative** result compared with an equal-budget label-blind uniform selection expectation at the reported 10% capacity setting. Two graph configurations respond differently.

The results do not establish a new classifier, an improved review policy, field energy savings, causal attribution to a single physical transducer, or a universal rule across buildings. Real-building building-automation records and rooftop-unit analyses provide different, non-equivalent context, **not independent replication** of the simulated reheat-position-loss mechanism.

## What is publicly available

The existing `derived_results/` directory contains eight historical, non-restricted aggregate tables (S1–S8) from an earlier OIR-FDD evaluation. They **do not constitute a complete release of the present sensor-loss decision study**, and should not be described as its final Supplementary Tables or a complete reproduction of the current figures.

The existing `algorithms/`, `data_manifest/`, `manuscript/`, `supplementary/` and `reproducibility/` directories contain historical methodological specifications, provenance notes, or source snapshots. These are preserved for traceability; they are **not authoritative copies of the current IEEE Access manuscript and supplement**. Older references to OIR-FDD, IGTI and CRRA identify historical evidence-audit procedures, not newly validated classifiers or the main novel method of this manuscript.

The current authoritative manuscript, supplement, archived evaluation ledger and versioned analysis artifacts remain in the authors' controlled submission package. The public repository presently does **not** establish independently verified, end-to-end reproduction of the reported training, pairing, capacity-selection, and figure-generation pipeline.

## Data and release limitations

Third-party raw HVAC data are not redistributed here; acquire the applicable datasets from their original providers under the respective terms. The authors plan to release permissible author-controlled analysis code, configurations, manifests, frozen evaluation outputs and trained-model artifacts after manuscript acceptance, subject to licensing, author verification and availability. **This is a planned release, not a completed public reproducibility claim.**

## Citation and status

Please cite the associated manuscript once it has an authoritative publication record. The historical `CITATION.cff` metadata may not describe the current paper and should be read together with this README until updated. No final DOI or acceptance date has been assigned.

Repository scope updated 20 November 2026 for the manuscript revision.