# Exploring Gene Expression in Breast Cancer Samples from the TCGA-BRCA Cohort

**Author:** Jewel Irvin  
**Project:** Data Science Project with R
**Date:** October 18, 2026

## Overview

This project explores gene-expression patterns in breast cancer samples from the TCGA-BRCA cohort. The analysis focuses on **ESR1** as the primary gene of interest, **ERBB2** as a secondary gene, and PAM50 molecular subtype as a sample-level characteristic.

The project uses descriptive statistics and data visualizations to examine gene-expression distributions, compare selected genes, and explore patterns across molecular subtypes.

## Research Question

**How does ESR1 gene expression vary across breast cancer samples and PAM50 molecular subtypes?**

## Objectives

- Examine the distribution of ESR1 expression across samples.
- Calculate descriptive statistics for ESR1 and ERBB2.
- Visualize the relationship between ESR1 and ERBB2 expression.
- Compare ESR1 expression across PAM50 molecular subtypes.
- Explore expression patterns across ten selected genes.
- Describe the distribution of PAM50 subtypes represented in the dataset.

## Data

The analysis uses two course-provided files:

- `counts.csv` — gene-expression count matrix containing gene identifiers and expression measurements across samples.
- `meta_data.csv` — sample metadata containing PAM50 molecular subtype annotations.

The analysis identifies ESR1 and ERBB2 using their Ensembl gene identifiers and connects expression measurements with sample metadata for subtype comparisons.


## Methods

The project uses R for data preparation, descriptive statistics, and visualization.

The analysis includes:

1. **Data preparation:** Load the expression matrix and metadata, inspect their structure, and identify selected genes.
2. **Descriptive statistics:** Calculate the mean, median, standard deviation, minimum, and maximum expression counts for ESR1 and ERBB2.
3. **Data visualization:** Generate five plots to explore gene expression and sample characteristics.
4. **Interpretation:** Describe visible patterns and acknowledge limitations, including unequal sample counts across PAM50 subtypes.

## Visualizations

1. **ESR1 expression histogram** — examines the distribution of ESR1 expression across samples.
<img width="2400" height="1500" alt="esr1_histogram" src="https://github.com/user-attachments/assets/5bf8ed7d-3fdc-4c24-9dba-f6bb137f8d05" />

   
2. **ESR1 versus ERBB2 scatter plot** — compares expression levels of the two selected genes.

<img width="2400" height="1500" alt="esr1_erbb2_scatter" src="https://github.com/user-attachments/assets/86917df8-248c-45c8-a48b-e5de09b2c195" />

3. **ESR1 expression by PAM50 subtype** — compares expression distributions across Basal, HER2-enriched, Luminal A, Luminal B, and Normal-like groups.

<img width="2400" height="1500" alt="esr1_pam50_boxplot" src="https://github.com/user-attachments/assets/a9342679-b73d-4733-b9eb-8b615dfd0400" />

4. **Ten-gene expression heatmap** — visualizes expression patterns across selected genes and samples, with PAM50 subtype annotations.

<img width="1400" height="865" alt="heatmaps1" src="https://github.com/user-attachments/assets/bc23e168-9235-4e0f-82b5-c522155789b1" />


5. **PAM50 subtype bar chart** — displays the number of samples in each molecular subtype.

<img width="2400" height="1500" alt="heatmap" src="https://github.com/user-attachments/assets/546b9fb9-9d9c-4539-9f0e-cfffb5fc22ef" />

## Key Findings

- ESR1 expression has a right-skewed distribution, with most samples showing comparatively lower counts and a smaller number showing substantially higher counts.
- ESR1 and ERBB2 exhibit considerable variation in expression across samples. Additional statistical analysis would be needed to quantify their relationship.
- ESR1 expression distributions can be visually compared across the five PAM50 molecular subtypes.
- The heatmap provides a broader view of expression patterns across ten selected genes.
- Luminal A is the most represented PAM50 subtype, with 571 samples, while Normal-like is the least represented, with 40 samples.





## Limitations

- The analysis is primarily descriptive and visual.
- The relationship between ESR1 and ERBB2 is not established through formal statistical testing.
- PAM50 groups have unequal sample sizes, which can affect the stability of comparisons.
- Visual patterns alone cannot establish causal relationships or clinical implications.
  

## References

- Course instructor. (2026). `counts.csv`. Course-provided gene-expression count matrix.
- Course instructor. (2026). `meta_data.csv`. Course-provided sample metadata.
- OpenAI. (2026). ChatGPT. Used for coding assistance and troubleshooting, as acknowledged in the project report.

