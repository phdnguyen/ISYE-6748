# Patient Cost of Care Drivers

Exploratory analysis and modeling to understand what factors drive patient cost of care.

## Goals
- Identify major contributors to cost (utilization, conditions, demographics, network, etc.)
- Build interpretable models for cost prediction / attribution
- Produce reproducible notebooks and report-ready outputs

## Data Safety
Raw and sensitive datasets must NOT be committed to git.
See `.gitignore` (data/raw and data/interim are ignored).

## Setup
```bash
conda env create -f environment.yml
conda activate data_6748
```

## Directory tree

```
.
├── data
│   ├── interim
│   ├── processed
│   └── raw
│       ├── ehn_gt_inpatient_20251223000.csv
│       ├── ehn_gt_outpatient_20251223000.csv
├── environment.yml
├── LICENSE
├── notebooks
│   ├── 01_eda.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_modeling.ipynb
│   └── test.ipynb
├── output
│   ├── figures
│   └── tables
├── README.md
└── src
    └── config.py
```