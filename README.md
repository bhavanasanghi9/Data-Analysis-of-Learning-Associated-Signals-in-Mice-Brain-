# Data-Analysis-of-Learning-Associated-Signals-in-Mice-Brain-
Analysis of large-scale spatial transcriptomics and single-nucleus RNA-seq data to study hippocampal activity patterns using Python, Scanpy, and statistical methods.

# Large-Scale Genomic Data Analysis: Spatial Object Recognition in Hippocampal CA3
## Project Question
Are specific transcriptional programs in CA3 hippocampal neurons associated with encoding spatial object recognition memory, and how are these programs spatially organized across hippocampal subregions in trained (SOR) vs. control (HC) mice?

# Overview
This project analyzes spatial transcriptomics (Visium) and single-nucleus RNA-seq (snRNA-seq) datasets to investigate how hippocampal CA3 neurons encode spatial object recognition (SOR) memory. Using Python and Scanpy, the pipeline processes ~14 tissue datasets (~50k features each) and thousands of single-nucleus profiles to identify activity-related transcriptional changes and their spatial localization across hippocampal subregions.The work demonstrates skills in data cleaning, normalization, dimensionality reduction (PCA, UMAP), statistical testing, and multi-modal data integration.

# Tech Stack
Programming: Python, Jupyter
Libraries: Scanpy, Pandas, NumPy, Matplotlib/Seaborn
Methods: Quality Control (QC), Normalization, PCA, UMAP, Mann–Whitney U Test, Cosine Similarity, Spearman Correlation
Data Types: Spatial Transcriptomics (Visium), snRNA-seq

# Methods
## Preprocessing & QC
Filtered low-quality spots/cells.
Normalized counts across datasets.
## Dimensionality Reduction
Applied PCA for variance capture.
Used UMAP for visualization of high-dimensional structure.
## Statistical Analysis
Mann–Whitney U tests to compare trained (SOR) vs control (HC) groups.
Cosine similarity to align Visium spots with snRNA-seq CA3 references.
Spearman correlation to assess activity vs. identity shifts.
## Integration
Combined ~11,000 shared genes across spatial and snRNA-seq datasets.
Linked cell-type identity with transcriptional activity patterns.

# Results
1. Activity-linked genes (Fos, Arc, Egr1) were strongly upregulated in trained samples (p < 1e-11).
2. Spatial clustering of gene activation observed in CA3, consistent with localized “engram”-like neuronal ensembles.
3. Cosine similarity analysis showed no stable identity shifts between groups.
Spearman correlation (ρ ≈ –0.39, p ≈ 4.6e-8) revealed that transcriptional changes were activity-driven rather than identity-driven.

# Discussion
1. The CA3 subregion of the hippocampus contributes to pattern completion and associative memory through selective recruitment of neuronal ensembles.
2. This project provides molecular and spatial evidence that SOR training induces localized, reversible transcriptional activation in CA3 pyramidal neurons without altering their cell identity.
3. Beyond neuroscience, this pipeline demonstrates the application of scalable data science methods to high-dimensional biological datasets, showcasing transferable skills in data preprocessing, dimensionality reduction, statistical testing, and multi-modal integration.

