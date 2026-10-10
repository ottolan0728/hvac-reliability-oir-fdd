# CRRA — Class-Retention Reliability Audit

CRRA audits whether aggregate calibration or selective-risk improvements remain
credible after fault-class retention and persistent sensor-loss stress are considered.

```text
evaluate raw and source-only calibrated probabilities

for each declared threshold or coverage slice:
    compute aggregate risk and coverage
    compute class coverage, accepted recall, and end-to-end recall
    if low aggregate risk coincides with zero accepted support
       for maintenance-relevant fault classes:
        flag SELECTIVE_CLASS_COLLAPSE

for each persistent sensor-dropout condition:
    evaluate BA, macro-F1, ECE, and AURC
    evaluate source-governed fallback under the same condition

if an aggregate gain is contradicted by class-retention collapse
   or adverse worst-condition sensor stress:
    do not promote it to a reliability gain
```
