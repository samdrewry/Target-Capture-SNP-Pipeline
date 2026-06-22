# Target Capture SNP Pipeline

This repository contains a reproducible bioinformatics workflow for processing target-capture sequencing data and analyzing SNP variation. The pipeline is written as an R Markdown tutorial and is intended to guide users through read quality assessment, trimming, alignment, SNP calling, filtering, and downstream population genomic analyses.

## Project Overview

This workflow was developed for target-capture population genomic data generated using the Compositae-1061 probe set. The pipeline includes steps for:

* Evaluating raw read quality
* Removing adapters and low-quality reads
* Aligning reads to a reference genome
* Calling and filtering SNPs
* Preparing datasets for downstream population genomic analyses
* Running PCA, ADMIXTURE, TreeMix, and D- and f-statistics analyses

## Repository Structure

```text
Target-Capture-SNP-Pipeline/
├── figures/           # Figures generated from analyses
├── docs/              # Rendered files for GitHub Pages
├── index.Rmd          # Main R Markdown tutorial
└── README.md          # Repository overview
```

## Getting Started

Clone the repository:

```bash
git clone https://github.com/samdrewry/Target-Capture-SNP-Pipeline.git
```

Open the project folder in RStudio and render the main R Markdown file:

```r
rmarkdown::render("index.Rmd")
```

## Required Software

This workflow uses a combination of command-line and R-based tools, including:

* FastQC
* MultiQC
* Trimmomatic
* Bowtie2
* SAMtools
* BCFtools
* PLINK
* ADMIXTURE
* TreeMix
* Dsuite
* R and RStudio

Additional R packages are listed within the R Markdown tutorial.

## Citation

If using this workflow, please cite the associated manuscript or repository. Citation information will be added here once available.

## Contact

For questions about this pipeline, please contact:

Samantha G. Drewry
Erika R. Moore-Pollard
Jennifer R. Mandel
