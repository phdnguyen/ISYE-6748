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