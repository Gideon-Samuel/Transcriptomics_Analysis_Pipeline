# Transcriptomics Analysis Pipeline

> A reproducible transcriptomic analysis workflow implemented in R.

## Overview

This repository contains an end-to-end transcriptomic analysis pipeline for gene expression data, supporting both microarray and RNA-seq datasets. The workflow includes differential expression analysis, gene annotation, visualization, and functional enrichment.

---

## Pipelines

### 1. LIMMA Pipeline (Microarray)

* Data retrieval from GEO
* Data preprocessing and normalization
* Quality control (PCA)
* Differential expression analysis using LIMMA
* Identification of significant genes (FDR < 0.05, |logFC| > 1)
* Probe-to-gene annotation
* Visualization:

  * PCA plot
  * Volcano plot
  * Heatmap
  * Sample clustering
* Functional enrichment:

  * Gene Ontology (GO)
  * KEGG pathways

---

### 2. DESeq2 Pipeline (RNA-seq)

*(To be added)*

---

## Dataset

* GEO Accession: GSE19188 (microarray)

---

## Project Structure

```
scripts/   → analysis pipelines  
results/   → output files (CSV, plots)  
```

---

## Tools Used

* R
* limma
* DESeq2
* GEOquery
* clusterProfiler
* org.Hs.eg.db
* ggplot2
* pheatmap

---

## Notes

* Gene-level expression is derived from probe-level data by selecting the most significant probe per gene.
* Statistical significance is determined using adjusted p-values (FDR).

---

## Author

Gideon Samuel
