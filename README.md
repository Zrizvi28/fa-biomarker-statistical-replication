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

The strongest finding is an ISG15-associated methylation signal. Two neighboring CpGs upstream of ISG15 showed directionally consistent hypomethylation across the infant and adolescent cohorts. The adolescent RNA-seq data also showed decreased ISG15 expression, providing additional biological support.

RGS14 was also identified as a candidate and is retained as an exploratory finding. However, the evidence for RGS14 is not strong enough to describe it as a validated or independently replicated biomarker.

The methylation and regional findings should therefore be considered candidates for future validation, particularly because several results do not remain significant after multiple-testing correction.

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

