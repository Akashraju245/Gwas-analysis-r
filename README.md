# 🧬GWAS Data Exploration using R

A simple, robust R script for exploring Genome-Wide Association Study (GWAS) data — load a TSV dataset, automatically detect the p-value column, and visualize the distribution of GWAS p-values.

![R](https://img.shields.io/badge/R-4.0%2B-276DC3?logo=r&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Active-success)

---

## 📖Overview

This project provides a lightweight workflow for exploring GWAS summary statistics. It focuses on **safely loading messy, real-world GWAS data** and producing a clear visualization of the p-value distribution — a common first step before deeper downstream analysis (e.g., Manhattan plots, QQ plots, or significance filtering).

## ✨Features

- 📂 **Robust TSV loading** — reads GWAS data even with inconsistent column formatting
- 🔍 **Automatic p-value column detection** — no need to hardcode column names
- 🔢 **Numeric conversion** — cleans and converts p-values to numeric format for analysis
- 📊 **P-value distribution plot** — generates and saves a histogram of p-values
- ⚙️ **CI workflow included** — repository includes a GitHub Actions workflow for automation

## 🛠️Requirements

- R 4.0 or higher
- RStudio (optional, recommended for interactive use)

## 🚀Getting Started

### Installation

```bash
git clone https://github.com/Akashraju245/Gwas-analysis-r.git
cd Gwas-analysis-r
```

### Usage

1. Open **R** or **RStudio**
2. Set your working directory to the project folder:
   ```r
   setwd("path/to/Gwas-analysis-r")
   ```
3. Run the analysis script:
   ```r
   source("gwas_analysis.R")
   ```

The script will read `data.xlsx.tsv`, detect the p-value column, and output a p-value distribution plot.

## 📊 Output

Running the script produces a histogram of the GWAS p-value distribution, saved as a PNG file:

`pvalue_distribution.png`

An `.RData` file (`pvalue_distribution.RData`) is also saved, containing the processed data and plot object for further use in R.

## 📁Project Structure

```
Gwas-analysis-r/
├── .github/workflows/          # CI/CD automation
├── gwas_analysis.R             # Main R script — data loading & analysis
├── data.xlsx.tsv               # GWAS dataset (TSV format)
├── pvalue_distribution.png     # Output: p-value distribution histogram
├── pvalue_distribution.RData   # Output: saved R data/plot object
└── README.md                   # Project documentation
```

## 🗺️Roadmap

- [ ] Add Manhattan plot visualization
- [ ] Add QQ plot for p-value diagnostics
- [ ] Support filtering by significance threshold (e.g., genome-wide significance)
- [ ] Add unit tests / validation checks for input data
- [ ] Parameterize input/output file paths via command-line arguments

## 🤝Contributing

Contributions are welcome! If you'd like to improve this project:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m "Add your feature"`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

## 📄License

This project is open source. Consider adding a [LICENSE](LICENSE) 

## 👤Author

**Akashraju245**
GitHub: [@Akashraju245](https://github.com/Akashraju245)

---

⭐ If you found this project useful, consider giving it a star on GitHub!
