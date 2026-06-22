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

The rendered tutorial can be viewed online without downloading the repository or opening RStudio:

[View the Target Capture SNP Pipeline website](https://samdrewry.github.io/Target-Capture-SNP-Pipeline/)

Users who want to inspect the source files, modify the workflow, or run the R Markdown document locally can clone the repository:

```bash
git clone https://github.com/samdrewry/Target-Capture-SNP-Pipeline.git
```

After cloning, open the project folder in RStudio by selecting:

```text
File > New Project > Existing Directory
```

and choosing the `Target-Capture-SNP-Pipeline/` folder.

The main tutorial file is:

```text
index.Rmd
```

To render the tutorial locally, run:

```r
rmarkdown::render("index.Rmd")
```

This will generate the rendered HTML file:

```text
index.html
```

which is the file used for the GitHub Pages website.

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
