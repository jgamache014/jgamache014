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
