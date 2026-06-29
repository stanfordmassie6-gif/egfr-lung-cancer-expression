# EGFR Expression in Lung Adenocarcinoma

## Question
Is EGFR differentially expressed between primary lung tumor tissue and adjacent normal tissue?

## Data
GSE32863 (NCBI GEO) — 116 lung tissue samples (58 tumor, 58 normal), Illumina microarray

## Methods
- Loaded and parsed GEO dataset using GEOparse
- Averaged expression across 4 EGFR probes for robustness
- Compared tumor vs normal using independent t-test
- Visualized distributions with boxplot and violin plot

## Result
EGFR is significantly upregulated in lung adenocarcinoma vs normal tissue 
(p = 1.32e-06). Tumor samples show substantially greater variance, consistent 
with known EGFR amplification heterogeneity in NSCLC.

## Tools
Python, pandas, seaborn, matplotlib, scipy, GEOparse
