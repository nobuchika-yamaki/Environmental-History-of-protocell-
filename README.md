# Reviewer Code Package

This package contains three self-contained Python scripts used for the fixed 10-hole environmental-history protocell analysis.

## Files

### 1. PROTOCELL_MAIN_ANALYSIS.py

Main analysis pipeline.

This script runs the primary fixed 10-hole simulation, performs the main post hoc analyses, computes EII and IRI outputs, and generates the manuscript figures.

### 2. PROTOCELL_SEED_ANALYSIS.py

Seed-replication analysis.

This script performs the N10 seed-replication analysis using the same fixed 10-hole formation protocol and six open-sea environmental histories.

### 3. PROTOCELL_SENSITIVITY_ANALYSIS.py

Coefficient-sensitivity analysis.

This script performs the coefficient-sensitivity analysis by perturbing formation, internal-state, and environmental coupling parameters.

## Suggested order

1. Run PROTOCELL_MAIN_ANALYSIS.py
2. Run PROTOCELL_SEED_ANALYSIS.py
3. Run PROTOCELL_SENSITIVITY_ANALYSIS.py

## Notes

Each script is self-contained and embeds the required internal source code. No additional Python source files are required. The seed-replication and coefficient-sensitivity scripts are robustness analyses and do not replace the main EII and IRI analyses.

