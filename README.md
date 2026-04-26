# AF-Metabolism-Stroke-MR

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Overview
This repository contains the analytical pipeline for the study: **"Metabolomic Profiling Identifies Histidine Depletion in Atrial Fibrillation Microenvironment as a Causal Risk Factor for Cardioembolic Stroke: Insights for Cardiovascular Nursing."**

The project integrates secondary metabolomic data mining with two-sample Mendelian Randomization (MR) to identify modifiable metabolic targets for stroke prevention in Atrial Fibrillation (AF) patients.

## Key Findings
- **Metabolomic Reprogramming:** Exposure to the AF microenvironment (AF-EAT) significantly alters amino acid metabolism in lymphatic endothelial cells (LECs).
- **Histidine Depletion:** Histidine was identified as a core depleted metabolite in the AF microenvironment.
- **Causal Evidence:** Two-sample MR analysis confirmed that lower circulating histidine levels are causally linked to an increased risk of cardioembolic stroke (OR = 0.716, P = 0.024).

## Repository Structure
- `code.R`: The integrated R script containing data cleaning, differential analysis, and Mendelian Randomization pipelines.
- `data/`:
  - `Significant_Metabolites_for_MR.csv`: The bridge file containing significantly altered metabolites used for causal inference.
- `Supplementary_Table_S1.xlsx`: Comprehensive data sheets for the manuscript.

## Environment & Requirements
The analysis was performed using **R version 4.3.1**. The following R packages are required:
- `TwoSampleMR`
- `dplyr`
- `ggplot2`
- `patchwork`

## How to Reproduce
1. Clone this repository to your local machine.
2. Ensure all required R packages are installed.
3. Run the `code.R` script. The script uses relative paths to load data from the `data/` folder.

## Data Sources
- **Metabolomics:** NIH Common Fund's National Metabolomics Data Repository (Study ID: ST004739, DOI: 10.21228/M8085J).
- **GWAS Statistics:** IEU OpenGWAS project (Exposure: met-a-495; Outcome: ebi-a-GCST006908).

## Acknowledgements
We thank the original investigators of the ST004739 dataset and the IEU OpenGWAS team. Special thanks to **Dr. Bing Tang** (Department of Integrated Traditional Chinese and Western Medicine Surgery, West China Hospital, Sichuan University) for methodological guidance.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
