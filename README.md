# Statistical Analysis of High-Throughput Genomic and Transcriptomic Data
Fall/Herbst-semester 2022

## Lectures
Mondays 9.00-9.45 (Y27-H-46), 10.00-10.45 (Y27-H-46)

## Exercises
Monday 11.00-11.45 (Y01-F-50)

## Lecturers

[Dr. Hubert Rehrauer](http://www.fgcz.ch/the-center/people/rehrauer.html), Group Leader of Genome Informatics at [FGCZ](http://www.fgcz.ch/)  

[Prof. Dr. Mark Robinson](https://robinsonlabuzh.github.io/), Associate Professor of Statistical Genomics, [DMLS](https://www.mls.uzh.ch/en.html), UZH  

[Emanuel Sonder](https://www.mls.uzh.ch/en/research/robinson/groupmembers/emanuel-sonder.html), PhD Student, [D-HEST](https://hest.ethz.ch/en), ETHZ  

[Helena Crowell](https://robinsonlabuzh.github.io/people.html), PhD Student, [DMLS](https://www.mls.uzh.ch/en.html), UZH  

[Anthony Sonrel](https://www.mls.uzh.ch/en/research/robinson/groupmembers/anthony-sonrel.html), PhD Student, [DMLS](https://www.mls.uzh.ch/en.html), UZH  

## Schedule

| Date  | Lecturer | Topic | Exercise | JC1 | JC2 |
| --- | --- | --- | --- | --- | --- |
| 19.09.2022  | Mark + Hubert  | admin; mol. bio. basics | quarto; git(hub) | | |
| 26.09.2022  | Mark | interactive technology/statistics session  | group exercise: technology pull request | | |
| 03.10.2022  | Hubert | NGS intro; exploratory data analysis | EDA in R | | |
| 10.10.2022  | Mark | limma + friends | linear model simulation + design matrices | | |
| 17.10.2022  | Hubert | mapping  | Rsubread | | |
| 24.10.2022  | Hubert | RNA-seq quantification | RSEM  | X | X |
| 31.10.2022  | Mark | edgeR+friends 1 | basic edgeR/voom | [Cell2location maps fine-grained cell types in spatial transcriptomics](https://www.nature.com/articles/s41587-021-01139-4) (JS, GM)  | [SPOTlight: seeded NMF regression to deconvolute spatial transcriptomics spots with single-cell transcriptomes](https://academic.oup.com/nar/article/49/9/e50/6129341) (PWG, FP) |
| 07.11.2022  | Emanuel | hands-on session #1: RNA-seq | FASTQC/Salmon/etc. | [Slingshot: cell lineage and pseudotime inference for single-cell transcriptomics](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-018-4772-0) (GB, ML)| [Capturing Heterogeneity in Gene Expression Studies by Surrogate Variable Analysis](https://journals.plos.org/plosgenetics/article?id=10.1371/journal.pgen.0030161) JK DW |
| 14.11.2022  | Mark | edgeR+friends 2  | advanced edgeR/voom | [Identifying gene expression programs of cell-type identity and cellular activity with single-cell RNA-Seq](https://elifesciences.org/articles/43803) (LM, YM) | [EAGLE: Explicit Alternative Genome Likelihood Evaluator - BMC Medical Genomics](https://bmcmedgenomics.biomedcentral.com/articles/10.1186/s12920-018-0342-1) (EJ, SL) |
| 21.11.2022  | Hubert | single-cell 1: preprocessing, dim. reduction, clustering | clustering | X | [Comparison of Transformations for Single-Cell RNA-Seq Data](https://www.biorxiv.org/content/10.1101/2021.06.24.449781v3.full.pdf) (GA, RE)|
| 28.11.2022 | Mark/Helena | hands-on session #2: cytometry | cytof null comparison | [Integrated analysis of multimodal single-cell data](https://www.sciencedirect.com/science/article/pii/S0092867421005833) (ME, FR) | [Moderated estimation of fold change and dispersion for RNA-seq data with DESeq2](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-014-0550-8) (KvG, AA) |
| 05.12.2022  | Mark | single-cell 2: clustering, marker gene DE  | marker gene DE | [Differential abundance testing on single-cell data using k-nearest neighbor graphs](https://www.nature.com/articles/s41587-021-01033-z) (DK) |[Redefining CpG islands using Hidden Markov Models](https://academic.oup.com/biostatistics/article/11/3/499/256898) (LL, JF)
| 12.12.2022  | Anthony | hands-on session #3: single-cell RNA-seq (cell type definition, differential state)  | full scRNA-seq pipeline | X | [Removing unwanted variation from large-scale RNA sequencing data with PRPS](https://www.nature.com/articles/s41587-022-01440-w)  (VH, MP) |
| 19.12.2022  | Mark | spatial omics  | spatial statistics | X | X |
 

## Course material

Assuming you have git installed locally, you can check out the entire set of course materials with the following command (from command line):
```
git clone https://github.com/sta426hs2022/material.git
```  
and get updates by running `git pull` at any later time in the same directory.

Alternatively, to retrieve a ZIP file of the repository, you can click on the (green) 'Code' button (top right of main panel) and then click 'Download ZIP'.
