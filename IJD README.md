# Targeting the upstream AIF1/IL6R axis in inflammatory joint diseases

This repository contains the custom R scripts and analytical pipelines used in the manuscript: 
**"Targeting the upstream AIF1/IL6R axis provides a cross-disease therapeutic bypass for inflammatory joint diseases: a multivariate genomic and functional study"** (Currently under review at *Nature Communications*).

## Project Overview
This project utilizes a multivariate Genome-Wide Association Study (GWAS) framework, Mendelian Randomization (MR), and single-cell RNA sequencing (scRNA-seq) to map the shared genetic architecture across the Inflammatory Joint Disease (IJD) spectrum. 
The pipeline prioritizes core causal genes (such as AIF1 and IL6R) and validates their specific expression and regulatory networks within monocytic populations.

## System Requirements
* **Operating System:** Tested on Windows 11 Pro (64-bit).
* **Software:** R version 4.5.2 
* **Hardware Requirements:** Tested on a local workstation equipped with an Intel Core i7-14700KF processor, 64.0 GB RAM, and an NVIDIA GeForce RTX 5070 (12 GB) GPU. While a minimum of 16GB RAM is required, 64GB RAM is highly recommended for efficient scRNA-seq matrix integration and high-dimensional Genomic SEM analyses.

## Dependencies and Installation
The following primary R packages are required to run the scripts. Typical installation time on a standard desktop computer is approximately [e.g., 30-60] minutes.

```R
# Key packages used in this pipeline:
install.packages(c("Seurat", "Harmony", "TwoSampleMR", "coloc"))
# Additional specialized packages:
# GenomicSEM (v.0.0.5), echolocatoR (v.2.0.3), ScPagwas