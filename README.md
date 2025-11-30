# **Spatial Transcriptomics in Alzheimer’s Disease (BDSI 2024)**

This repository contains code I developed during the **Big Data Summer Institute (BDSI)** at the **University of Michigan**. I worked in the Genomics group on a spatial transcriptomics project analyzing gene expression patterns across anatomical (white and gray matter) regions of post-mortem Alzheimer’s disease (AD) brain tissue.

The code in this repository represents **my individual contributions** to the project, which include:

- **Demographics cleaning and summary scripts**
- **Differential expression (DEG) pipeline**
- **Spatially varying gene (SVG) pipeline**
- **Graphing and visualization utilities**


---

## **Project Background**

Our group studied spatial transcriptomics data from a post-mortem Alzheimer’s dataset originally published in *Nature*. After reviewing the paper and related literature, we defined a shared analytical workflow focused on differential expression, spatial variation, and pathway-level analysis.

---

## **My Contributions**

### **Differential Expression (DEG) Pipeline**

I implemented the DEG pipeline using **edgeR** on pseudo-bulk aggregated data.

**Highlights:**
- Controlled for confounders such as age (control samples were roughly 10 years younger than AD groups).
- Identified most DEGs in gray-matter regions, especially **L3/4**.
- Pathway analysis (via **fgsea**) showed enrichment related to mitochondrial dysfunction, cytoskeletal organization, and cell-fate processes, consistent with known gray-matter decline in AD.

---

### **Spatially Varying Genes (SVG) Pipeline**

I independently wrote and ran the entire SVG analysis pipeline, selected significant results, and interpreted spatial expression patterns.

These spatial patterns illustrate localized dysregulation associated with disease progression.

---

### **Graphing and Demographic Analyses**

I created scripts for:
- Cleaning demographic metadata and summarizing variables such as age and disease stage
- Visualizing region-level gene expression
- Plotting DEG and SVG results


---

## **Note**

Raw data is **not** included due to licensing restrictions.
