# Hur Lab FoxP3 Paper Repository

This repository contains all Jupyter notebooks and custom scripts used in our FoxP3 motif enrichment and genomic co-occurrence study. Each notebook includes sample inputs, expected outputs, and demo runs.

All scripts are written in Python and are executable via Jupyter Notebook. They can be run on any platform (Windows, macOS, Linux) with a working Python environment.

To install Jupyter Notebook, see:  
https://jupyter.org/install

## Repository Overview

The repository is organized by figure, with each folder corresponding to a figure in the manuscript and the analysis pipeline used to generate it.

### `Figure1` – Paired-End Reads: Trimming, Motif Enrichment, and Visualization

This notebook processes paired-end PD-seq reads. It includes:
- Trimming reads to match the oligo structure
- Filtering based on read quality
- Counting and summarizing 7-mer sequences
- Calculating enrichment for FoxP3 binding
- Visualizing enrichment trends across replicates

### `Figure2` – Single-End Reads: Quality Control, Shifting, Bias Correction

This notebook handles single-end read processing, including:
- Trimming and read quality assessment
- Positional shifting of reads to correct for experimental bias
- Correction for theoretical sequence input bias
- Visualization of FoxP3 vs FoxP1 pull-down enrichment using heatmaps

### `Figure3` – Motif Discovery in Genomic Peaks and Gap Analysis

This notebook scans genomic peaks for candidate motifs. It performs:
- Motif searches in FoxP3-bound peak regions
- Enrichment calculations using the exact binomial test
- Motif pair gap analysis to detect enriched spatial arrangements

### `Figure4` – Identifying Valid TnG Repeats in H-T and T-H Motif Pairs

This notebook investigates which head-to-tail (H-T) and tail-to-head (T-H) motif pairs represent true TnG repeats. It includes:
- Sequence verification for repeat identity
- Filtering motif pairs based on TnG presence
- Classification of validated TnG motif combinations

### `Figure5` – Peak-Level Comparisons of H-H Motifs and TnG Repeats

This analysis explores spatial proximity between H-H motif pairs and TnG motifs in the genome. It includes:
- Comparison of FoxP3-bound versus FoxP3-free OCRs
- Distance calculations between motif pairs and TnG motifs
- Analysis of TnG locus length distributions based on proximity to motif pairs
