# Reviewer Code Package

This package contains the Python scripts used for the fixed 10-hole environmental-history protocell analysis.

## 1. FULL_OPEN_SEA_FIXED10HOLES_ENV_SWEEP.py

Main simulation script.

This script generates protocell-like components in a fixed 10-hole formation environment, releases the same component state into six open-sea environments, tracks component dynamics, and writes the primary CSV outputs used for analysis.

Main outputs include component time series, population diversity time series, component lineage/event data, and voxel snapshots.

## 2. POSTHOC_FIXED10_ENV_HISTORY_1TO4.py

Post hoc transformation analysis.

This script analyzes release-to-re-fusion changes across environments. It computes structural changes, trait-diversity exposure, re-fusion timing, fusion events, threshold sensitivity, and the Environmental Imprint Index (EII).

## 3. POSTHOC_IMPRINT_RETENTION_IRI.py

Post hoc imprint-retention analysis.

This script analyzes whether release-to-re-fusion changes remain in the final aggregate. It computes the Imprint Retention Index (IRI), retained-imprint scores, metric-level retention values, and retention classes.

## 4. GENERATE_FIXED10_ENV_HISTORY_PAPER_FIGURES_FIXED_LAYOUT.py

Figure-generation script.

This script generates the manuscript figures from the simulation and post hoc analysis outputs. It produces Figures 1–6 used in the manuscript.

## 5. N10_SEED_REPLICATION_FIXED10_ENV.py

Seed-replication analysis.

This script performs the N10 seed-replication analysis using the same fixed 10-hole formation protocol and six open-sea environments. It tests whether the main environment-dependent tendencies remain visible across stochastic seeds.

## 6. COEFFICIENT_SENSITIVITY_FIXED10_ENV_PARALLEL.py

Coefficient-sensitivity analysis.

This script performs a moderate coefficient-sensitivity analysis. It perturbs formation, internal-state, and environmental coupling coefficients and runs variants in parallel. It is used to test whether the qualitative results depend on a narrow hand-tuned parameter setting.

## Suggested analysis order

1. Run FULL_OPEN_SEA_FIXED10HOLES_ENV_SWEEP.py.
2. Run POSTHOC_FIXED10_ENV_HISTORY_1TO4.py.
3. Run POSTHOC_IMPRINT_RETENTION_IRI.py.
4. Run GENERATE_FIXED10_ENV_HISTORY_PAPER_FIGURES_FIXED_LAYOUT.py.
5. Run N10_SEED_REPLICATION_FIXED10_ENV.py.
6. Run COEFFICIENT_SENSITIVITY_FIXED10_ENV_PARALLEL.py.

## Notes

The main analysis is based on the fixed 10-hole formation run and the six open-sea environmental histories. The N10 seed-replication and coefficient-sensitivity scripts are robustness analyses and are not replacements for the main EII and IRI post hoc analyses.
