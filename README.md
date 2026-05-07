# Patient Cost of Care Drivers

Graduate practicum project (ISYE 6748 — Georgia Tech) analyzing inpatient and outpatient claims data to identify key drivers of patient cost of care.

## Overview

Using real-world claims data, we explore utilization patterns, diagnoses, demographics, and network factors to build interpretable cost prediction models. Separate analysis pipelines are maintained for inpatient and outpatient populations.

## Setup

```bash
conda env create -f environment.yml
conda activate data_6748
```

## Project Structure

```
.
├── data/
│   ├── raw/              # Source data (not committed)
│   ├── interim/          # Intermediate transformations (not committed)
│   └── processed/        # Final modeling-ready datasets
├── notebooks/
│   ├── 00_data_cleaning.ipynb
│   ├── 01_inpatient_EDA.ipynb
│   ├── 02a_inpatient_EDA.ipynb
│   ├── 03_totalcost_calibration.ipynb
│   ├── 03a_inpatient_baseline_models.ipynb
│   ├── 03b_inpatient_models_phase2.ipynb
│   ├── 03c_inpatient_models_phase3.ipynb
│   ├── 03d_inpatient_models_phase4.ipynb
│   └── Outpatient/
│       ├── 01_EDA_Outpatient_Data.ipynb
│       ├── 02_Feature_Engineering_Outpatient.ipynb
│       └── 03_EDA_Notebook_Outpatient.ipynb
├── output/
│   ├── figures/
│   └── tables/
├── src/
│   └── config.py
└── environment.yml
```

## Data

Raw data files are excluded from version control via `.gitignore`. Do not commit any files under `data/raw/` or `data/interim/`.
