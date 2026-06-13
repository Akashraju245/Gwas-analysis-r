# GWAS Data Exploration using R

This repository contains a R script for exploring Genome-Wide Association Study (GWAS) 
data stored in a TSV file.  
The project focuses on safely loading the data and visualizing the distribution of GWAS p-values.

---

## Repository Information

This repository contains scripts and workflows for Genome-Wide Association Study (GWAS) analysis, data processing, and result visualization using R.
## Files in this Repository
- `gwas_analysis.R` – R script for GWAS data loading and analysis  
- `data.xls.tsv` – GWAS dataset (TSV format)  
- `pvalue_distribution.png` – Histogram of GWAS p-value distribution  
- `README.md` – Project documentation  

---

## Analysis Performed
- Reads GWAS TSV file using a robust method  
- Handles inconsistent column formatting  
- Automatically detects the p-value column  
- Converts p-values to numeric format  
- Generates and saves a p-value distribution plot  

---

## How to Run the Script
1. Open **R** or **RStudio**
2. Set the working directory to this project folder
3. Run:
```r
source("gwas_analysis.R")
