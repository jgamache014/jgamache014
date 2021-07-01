# **BIO:**

### I am currently using single-nuclei genomics technology to understand mechanisms of gene dysregulation in neurodegenerative diseases. Below is a description of my repository containing the R script used to process a single-nuclei (sn)RNA-seq dataset from human brain tissue. This is a work-in-progress, so I welcome any feedback or questions.

### Email: jgamache014@gmail.com

# **PROJECTS:**

### [snRNA-seq workflow](https://github.com/jgamache014/snRNA-seq-workflow)

This repository contains R code mainly using the packages [Seurat](https://satijalab.org/seurat/) and [MAST](https://www.bioconductor.org/packages/release/bioc/html/MAST.html) to analyze snRNA-seq data from 24 human temporal cortex samples for a final count of >200,000 nuclei. Prior to using this pipeline, the raw sequencing data was pre-processed using Cell Ranger v4.0 (10X Genomics) to convert to FASTQ files, align to GRCh38, and generate count matrices. The workflow involves the following steps:

  * Generate Seurat objects and perform QC filtering
  * Perform SCT normalization and integrate the datasets
  * Use an annotated reference dataset to annotate cell types
  * Perform dimensional reduction (PCA & UMAP)
  * Conduct differential expression analyses in MAST

### [Alzheimer's GWAS 1Mb genes list](https://github.com/jgamache014/Alzheimers_GWAS_1Mb_genes_list)

This project supplements the snRNA-seq workflow to further investigate underlying regulatory mechanisms of late-onset Alzheimer's disease (LOAD). Here, [biomaRt](https://bioconductor.org/packages/release/bioc/html/biomaRt.html) is used to extract gene names in 1Mb genomic regions surrounding all known LOAD GWAS loci, based on the most recent GWAS meta-analysis to date ([Bellenguez et al., 2020](https://www.medrxiv.org/content/10.1101/2020.10.01.20200659v2.full-text)). 
