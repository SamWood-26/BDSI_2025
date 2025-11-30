Spatial Transcriptomics in Alzheimer’s Disease (BDSI 2024)

This repository contains code I developed during the Big Data Summer Institute (BDSI) at the University of Michigan. I was part of the Genomics group working on a spatial transcriptomics project analyzing gene expression patterns across anatomical(White and Gray matter) regions of post-mortem Alzheimer’s disease (AD) brain tissue.

The code in this repository represents my individual contributions to the project, which include:

Differential expression (DEG) pipeline

Spatially varying gene (SVG) pipeline

Graphing and visualization utilities

Demographics cleaning and summary scripts

Project Background

Our group studied spatial transcriptomics data from a post-mortem Alzheimer’s disease dataset originally published in Nature. After reviewing the paper and related literature, we defined a shared analytical workflow focused on differential expression, spatial variation, and pathway-level analysis.

My Contributions
Differential Expression (DEG) Pipeline

I implemented the DEG pipeline using edgeR on pseudo-bulk aggregated data.
Highlights:

Controlled for confounders such as age (control samples were roughly 10 years younger than AD groups).

Identified the majority of DEGs in gray matter regions, especially L3/4.

Follow-up pathway analysis (via fgsea) showed enrichment related to mitochondrial dysfunction, cytoskeletal organization, and cell-fate processes, consistent with known gray matter decline in AD.

Spatially Varying Genes (SVG) Pipeline

I independently wrote and ran the full SVG analysis pipeline, selected significant results, and interpreted spatial patterns.

Two main gene categories emerged:

Genes consistent in controls but region-specific in AD

Example: APLP1, linked to neurogenesis, became gray-matter-specific in AD.

Genes low in controls but highly region-specific in AD

Example: IFI35, involved in inflammation signaling, showed strong gray-matter overexpression in AD.

These patterns point to spatially localized dysregulation as the disease progresses.

Graphing and Demographic Analyses

I created scripts for:

Visualizing region-level gene expression

Plotting DEG and SVG results

Cleaning demographic metadata and summarizing factors such as age and disease stage

Note 

Raw data is not included
