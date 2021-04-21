# Comparison of algorithms used in single-cell biological analysis

## Abstract

Single-Cell Analysis is an increasingly relevant approach in "omics" studies. In the last decade, it has been applied to various fields, including cancer biology, neuroscience, and, especially, developmental biology. This rise in popularity has been accompanied with creation of modern software, development of new pipelines and design of new algorithms. Many established algorithms have also been applied with varying levels of effectiveness. Currently, there is abundance of algorithms for all steps of the general work flow. While some scientists use ready-made pipelines (such as Seurat), manual analysis is popular, too, as it allows more flexibility. Scientists who perform their own analysis face with multiple options when it comes to the choice of algorithms. We have used two different datasets to test some of the most widely-used algorithms. In this paper, we are going to report the main differences between them, suggest a minimal number of algorithms for each step, and explain our suggestions. In certain stages, it is impossible to make a clear choice without further context. In these cases, we are going to explore the major possibilities, and make suggestions for each one of them.

## Introduction
Quantitative analysis of cell contents - mostly DNA, RNA and protein - has been a major part of molecular biology since emergence of the field. Studying protein content of the cell is helpful when we are trying to uncover dynamics of its metabolism. Observing changes in DNA sequence through the generations allows us to understand the evolutionary processes at cell level. Comparing amount of different RNA molecules enables us to fill the gap between these two separate pieces of information by unveiling the expression patterns of the cell.  

Our report concentrates on single-cell RNA sequencing analysis - a revolutionary combination of molecular and computational techniques that opens up new dimensions in our understanding of tissues. Before we get started, it is important to understand both conceptual and technical differences between single-cell analysis and its traditional counterpart.

### The tradition: bulk analysis
Molecular analyses rely on sample abundance. In order to sequence a single gene, we need multiple copies. The same thing applies to RNA sequences, too. Amplification techniques such as PCR allows us to sequence small DNA and RNA samples. We can reproduce and sequence particular nucleic acids, but we can not reproduce individual cells. Instead, a tissue has to be assumed to be homogeneous and analyzed in bulk. The power of this approach lies in its simplicity - so does its weakness. Bulk analysis did, and still does, provide insightful information about expression levels of genes in a tissue. But this strips us of our ability to analyze cells individually. This limitation is not merely principal. It comes with a set of problems in our understanding of cell states. Simpson's Paradox is an interesting example to this. Only in 21st century did we start to approach these problem. Progress in molecular techniques, coupled with advances in computer science and information technologies set the stage for a new generation of analysis tools to be developed.

### The novelty: single-cell analysis
As a result of progress in amplification techniques and cell capture/isolation instruments, we are now able to perform RNA sequencing on individual cells. RNA-seq is not the only relevant method of measuring cell state. Others include Hi-C (method for measuring chromatin conformation), bisulfite sequencing, and DNase I hypersensitivity sequencing. Each one of these can now be performed i single-cell scale. However, single-cell RNA sequencing analysis has been our sole concentration through the program. Before reporting our research and findings, here is a brief introduction to the field.

### Single-cell RNA sequencing analysis
scRNA-seq analysis can be divided into two easily distinguishable states: pre-processing and downstream analysis.  receives raw data in one of several possible formats. 

...

### Analyzed Papers
Single-cell analysis has evolved into a considerably large field. As of April, 2020, there are more than 1200 articles in Single Cell Studies Database. We had to pick two different papers from this database, taking into account several factors:  
(1) The paper has to involve single-cell RNA sequencing analysis as one of its major tools of research. That is to say, scRNA-seq analysis has to lead to major findings in the context of the paper.
(2) Most, if not all stages of the scRNA-seq analysis pipeline has be present in the research. Visually no single research utilizes every single technique of scRNA-seq analysis, so it is more reasonable to choose our two papers to maximize the coverage.
(3) Single cell data has to be present, preferably in raw form. Count matrix, observations (cells) and variables (genes) constitute backbone of the scRNA-seq data. No analysis can be performed if even one of them is missing. Cell and gene annotation provide more opportunities for analysis, but they are not imperative.  
(4) The tools and platforms used in scRNA-seq analysis has to documented clearly. We need to replicate some of the results presented in the paper (e.g. cell clustering). But large-scale, especially machine learning algorithms, tend have stochastic element to them, which means that in order to get some sort of similarity between our results, we need to use exactly same tools. Otherwise we can end up with virtually distinct outcomes.

Vastness of the database allowed us some freedom of choice, which means our preferences also had considerable effect in the choice of papers. We ended up with these two:
- Longitudinal single-cell RNA sequencing of patient-derived primary cells reveals drug-induced infidelity:

  In this paper, authors use scRNA-seq to probe variants of chemo-resistance of in tumor cells.

- Cellular Heterogeneity and Lineage Restriction during Mouse Digit Tip Regeneration at SC Resolution:

  In this paper, authors use scRNA-seq to classify cells found in homeostatic (where there is no need for regeneration) and regenerating mouse digit tips.

## Bibliography
- Trapnell C (2015) Defining cell types and states with single-cell genomics.
- Luecken MD, Theis FJ (2018) Current best practices in single-cell RNA-seq analysis: a tutorial.
- Sharma A, et al. (2018) Longitudinal single-cell RNA sequencing of patient-derived primary cells reveals drug-induced infidelity in stem cell hierarchy.
- Johnson GL, Masias EJ, Lehoczky JA (2020) Cellular Heterogeneity and Lineage Restriction during Mouse Digit Tip Regeneration at Single-Cell Resolution.

