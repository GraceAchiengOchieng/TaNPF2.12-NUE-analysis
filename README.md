TaNPF2.12 Nitrogen Use Efficiency Analysis

This repository contains the full analysis pipeline for evaluating TaNPF2.12 haplotypes in relation to root traits, nitrogen use efficiency (NUE), and grain yield across two seasons and two field environments.

Included:

Multi-environment phenotype data

Promoter and coding SNPs (−88 and +4)

Automated haplotype extraction

Boxplots of key traits

Promoter × coding ANOVA

Reaction norms (plasticity)

PCA for trait clustering

Motif analysis (PLACE)

Extended root architecture analysis

Environment stability plots

Correlation matrices

Pipeline structure

data/ — raw phenotype and SNP data

scripts/ — full R script pipeline (01–11)

figures/ — output plots

results/ — ANOVA tables & numeric outputs

docs/ — promoter motif & alignment documents

Reproducibility

Run the pipeline in sequence:

source("scripts/01_load_packages.R")
source("scripts/02_load_data.R")
source("scripts/03_clean_merge.R")
source("scripts/04_trait_boxplots.R")
source("scripts/05_anova_models.R")
source("scripts/06_plasticity_slopes.R")
source("scripts/07_environment_stability.R")
source("scripts/08_pca_analysis.R")


Additional analysis:

source("scripts/09_root_architecture_extended.R")
source("scripts/10_trait_correlations.R")
source("scripts/11_environment_boxplots.R")
