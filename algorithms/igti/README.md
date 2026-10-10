# IGTI — Identifiability-Gated Transfer Interpretation

IGTI is a deterministic audit algorithm used by OIR-FDD to prevent source-limited
classes from being misreported as transfer failures.

## Output states

- `SOURCE_IDENTIFIABLE_TARGET_FAILURE`
- `SOURCE_WEAK_TARGET_WEAK`
- `INCONCLUSIVE_SUPPORT`

## Pseudocode

```text
for each class c:
    verify support and physical eligibility
    if support is insufficient:
        return INCONCLUSIVE_SUPPORT

    determine source_status(c)

    if source_status(c) == STRONG and target recognition is weak:
        return SOURCE_IDENTIFIABLE_TARGET_FAILURE

    if source_status(c) == WEAK and target recognition is weak:
        return SOURCE_WEAK_TARGET_WEAK

    return INCONCLUSIVE_SUPPORT
```
