# DNA_SIP_qPCR_analysis
R Markdown workflow for density-resolved DNA-SIP qPCR analysis

This repository contains an R Markdown workflow for analyzing DNA-SIP (Stable Isotope Probing) qPCR data from density gradient fractionation experiments. The script performs data cleaning, integration of qPCR results with density information, and visualization of relative copy number distributions across fractions.

## Contents
- `DNA_SIP_qPCR_analysis.Rmd` — main R Markdown script  
- (optional) CSV files with input data if you include them  

## Requirements
The script uses R (≥4.0) and the following R packages:  
- tidyverse  
- ggplot2  
- dplyr  
- patchwork  
- scales  
- ggtext  
- see  
- extrafont  

## Input files
The script expects three CSV input files:
1. **`1.RI_DNA_SIP_frac.csv`** — Refractive index values per fraction  
2. **`2.qPCR_data_DNA_SIP_frac.csv`** — qPCR results for each fraction  
3. **`3.Treatments.csv`** — metadata linking samples to treatments  

These files should be placed in the working directory (set in the script).  

## Output
- Cleaned and summarized qPCR results (`qPCR_means.csv`)  
- Density-resolved relative fraction plots for each treatment (PDF format)  

## Usage
1. Clone or download this repository.  
2. Place the input CSV files in the working directory defined in the script.  
3. Open `DNA_SIP_qPCR_analysis.Rmd` in RStudio.  
4. Knit the document to generate the analysis and plots.  

## Citation
If you use or adapt this workflow, please cite:  
*Justus Nweze. DNA SIP qPCR analysis, 2023.*  
