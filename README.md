# Food Allergy Biomarker Statistical Replication
### Zamin Rizvi '28

## Objectives

This project investigates molecular differences associated with food allergy using publicly available DNA methylation and RNA-seq datasets. Rather than focusing on classification, the project examines whether candidate biomarkers show consistent statistical and biological evidence across independent, age-differentiated cohorts.

## Motivation

Food allergy results from a complex interaction between the immune system, genetics, and environmental factors. DNA methylation provides one way to investigate molecular changes that may be associated with allergic disease.

I was interested in whether methylation signals in resting, naive CD4 cells from one food-allergy cohort could also be observed in an independent cohort with a different age group, and whether those signals could be supported by changes in gene expression.

## Research Question

Which DNA methylation differences are associated with food allergy, and which candidate signals show evidence of consistency across independent cohorts?

The analysis focuses on three GEO datasets:

* GSE114134: infant DNA methylation data
* GSE189148: adolescent resting DNA methylation data
* GSE189149: adolescent RNA-seq data

## Analysis
The project uses R, Python, Jupyter, and Bioconductor tools to perform:

* DNA methylation quality control
* Differential methylation analysis
* Cross-cohort comparison
* Regional methylation analysis
* RNA-seq analysis
* Candidate gene investigation

## Results

The strongest finding is an ISG15-associated methylation signal. Two neighboring CpGs upstream of ISG15, cg08469540 and cg25610492, showed direction-consistent hypomethylation in allergic samples across both the infant and adolescent cohorts.

The two-probe region also produced nominally significant results in both cohorts, with p = 0.0175 in GSE114134 and p = 0.00589 in GSE189148. Although these results did not remain significant after family-wise error correction, the consistency in direction and location taken with the permutation null results provide a strong candidate for further investigation.

The corresponding RNA-seq analysis provides additional biological support. In GSE189149, the region was associated with decreased ISG15 expression (log₂FC ≈ −0.926), closely matching the published estimate of −0.931.

RGS14 was also identified as a candidate during the analysis and is retained as an exploratory finding. While it does not have the same level of evidence as ISG15, it provides an additional candidate for future investigation.

Taken together, the results identify ISG15 as the strongest molecular candidate, supported by cross-cohort methylation concordance, regional analysis, and an independent transcriptomic signal. These findings remain exploratory and require validation in additional cohorts.

## Conclusions

The results suggest that the region surrounding ISG15 is a promising candidate for further investigation in food allergy. RGS14 provides an additional candidate signal, but requires further independent evidence.

Overall, this project emphasizes statistical consistency and biological interpretation rather than prediction, with the goal of distinguishing promising molecular signals from findings that require additional validation.

## Repo Structure
├── notebooks/ 

├── scripts/ 

├── data/ 

└── results/

## Project Status
This repository is a focused continuation of my original food-allergy biomarker project. The classification component has been removed so that the project can focus on statistical biomarker analysis and biological interpretation.

