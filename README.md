# World Happiness – Regional Interpretation of Well-Being

This repository contains the preprocessing pipeline for the World Happiness dataset used in the Data Visualisation coursework.

## Current Status

The preprocessing stage is **complete and locked**.  
All steps are reproducible and designed to minimise bias before analysis.

### What has been implemented

- **Column standardisation**  
  Renamed variables for clarity and consistency.

- **Temporal coverage assessment**  
  Evaluated year availability per country to understand reporting gaps.

- **Data-driven temporal filtering**  
  Selected an optimal contiguous time window and retained only countries with sufficient year coverage.

- **Structural data cleaning**
  - Removed countries with irreparable missingness (e.g. South Sudan).
  - Dropped variables with systemic regional gaps (e.g. corruption).

- **Within-country interpolation**  
  Applied linear interpolation across time for numeric indicators, strictly within each country.

- **Transparency & reproducibility**
  - Final cleaned dataset exported (`world_happiness_final.csv`)
  - All excluded country-level records preserved separately (`excluded.csv`)

The preprocessing decisions are visualised and justified within the notebook to ensure clarity and auditability.

## Next Steps (Coming Soon)

- Exploratory Data Analysis (EDA)
- Definition of final research questions
- Visualisation-driven analysis and interpretation
- Storytelling and discussion aligned with coursework requirements

---

This repository will be updated incrementally as analysis progresses.
