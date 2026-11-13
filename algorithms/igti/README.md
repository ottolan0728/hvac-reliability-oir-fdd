# IGTI — Identifiability-Gated Transfer Interpretation

IGTI is a deterministic post-evaluation interpretation procedure. It does not fit to target labels or change classifier predictions.

For each retained class, independently evaluate source-test and target class precision/recall across the three source-selected model families (five-seed means). The frozen support guard requires at least 30 eligible class windows and five nonoverlapping 300-minute supports in **both** domains.

Domain state:
- **STRONG:** at least two families have recall >= 0.70 and precision >= 0.50.
- **WEAK:** at least two families have recall < 0.50.
- **UNRESOLVED:** all remaining situations.

The interpretation rules, after support passes, are:
- STRONG source / WEAK target -> `SOURCE_IDENTIFIABLE_TARGET_FAILURE`
- WEAK source / WEAK target -> `SOURCE_WEAK_TARGET_WEAK`
- STRONG source / STRONG target -> `SOURCE_STRONG_TARGET_STRONG`
- All other patterns -> `INCONCLUSIVE_SUPPORT`

If the count/support guard fails, also return `INCONCLUSIVE_SUPPORT`. The last output is therefore a catchall interpretation, not exclusively a statement that sample size is insufficient. Cutoffs are frozen empirical protocol choices, not physical guarantees.

See the manuscript's Algorithm 1 and supplementary class-support records for exact definitions. This README documents the published interpretation contract; it is **not** a validated executable implementation.
