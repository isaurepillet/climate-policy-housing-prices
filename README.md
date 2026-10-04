# Climate Policy and Housing Prices

**Applied econometrics project conducted with Forvis Mazars — ENSAE Paris**

This project studies how the **French Climate and Resilience Law (2021)** affected the valuation of energy-inefficient housing. It combines property transactions from **DVF (Demandes de valeurs foncières)** with **DPE (Diagnostic de performance énergétique)** data.

## Research question

Did the introduction of restrictions targeting energy-inefficient dwellings change their transaction prices relative to more energy-efficient properties?

The empirical analysis defines treatment groups from DPE ratings and compares price dynamics before and after **24 August 2021** using **Difference-in-Differences** specifications. In the main saved specification, dwellings rated **E, F or G** are assigned to the treated group and ratings **A–D** to the comparison group.

## Empirical workflow

The project required:

- cleaning and harmonising large DVF and DPE datasets;
- normalising addresses and matching property transactions to energy-performance records;
- analysing the distribution of DPE ratings before and after matching;
- constructing treatment, control and post-policy indicators;
- estimating hedonic price regressions and Difference-in-Differences models;
- adding property and geographic controls and performing robustness analyses.

## Main notebooks

The repository preserves the notebooks from the collaborative research workflow. The most useful entry points are:

- **`01_data_preparation.ipynb`** — preparation and harmonisation of DPE and property-transaction data;
- **`02_dvf_dpe_matching.ipynb`** — address normalisation and DVF–DPE matching;
- **`03_exploratory_analysis.ipynb`** — exploratory analysis of the source data;
- **`04_econometric_analysis.ipynb`** — construction of treatment/control groups and main econometric analysis.

Other notebooks are retained as intermediate collaborative work and robustness explorations.

## Data

The repository includes matched annual extracts used by the notebooks. The underlying public sources are:

- **DVF** — French property transactions;
- **DPE** — energy-performance certificates.

Some data-preparation notebooks were originally run in an ENSAE data environment and therefore contain environment-specific paths or S3 access code. The final matched extracts included here allow the modelling notebooks to document the empirical analysis without access to that environment.

## Tools and methods

Python · pandas · statsmodels · Jupyter · data matching · hedonic regressions · Difference-in-Differences

## Context

ENSAE Paris — *Statistique appliquée*  
Partner: **Forvis Mazars**
