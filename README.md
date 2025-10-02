# TELS1 and Cancer – GDC Data Re-analysis

This repository contains an RMarkdown-based re-analysis of public TCGA/GDC datasets, focusing on human **TELS1** (ENSG00000121903) and related genes such as TRF2, ATRX, and DAXX, in sarcoma cohorts.  
The goal is to provide a transparent, fully reproducible workflow and interactive figures (Kaplan–Meier curves, expression plots, clinical correlations, etc.).

---

## Contents

- `GDC-cancer-and-TELS1.html`  
  Interactive HTML report with:
  - Sample/sample correlations
  - Expression analysis of lineage controls (ACTA2, ATRX, DAXX)
  - Survival analyses (Kaplan–Meier, Cox models)
  - Combined TELS1/TRF2 expression patterns
  - Clinical associations (stage, diagnosis, survival, age, gender, etc.)
  - Interactive plots with **plotly** and **DT tables**

- `R/` and `.Rmd` scripts  
  Source code to regenerate the HTML analysis.

- `renv.lock`  
  Snapshot of the R environment for reproducibility.

---

## Reproducibility

The analysis is fully reproducible with [`renv`](https://rstudio.github.io/renv/).

## Website

[Access the website here](https://joeydufourd.github.io/TELS1-and-cancer/GDC-cancer-and-TELS1.html).

Clone the repository and restore the environment:

```bash
git clone https://github.com/joeydufourd/tels1-gdc-analysis.git
cd tels1-gdc-analysis
R -e "renv::restore()"
