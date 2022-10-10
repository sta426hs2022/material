# MERFISH (multiplexed error-robust fluorescence in situ hybridization)
***
Basic Idea: To quantify mRNA transcript spatially inside fixated cells (in situ) by hybridization of the mRNA with labeled complementary RNA probes. ([Source](https://doi.org/10.1186/s13073-022-01075-1))

## What does the method:

- Like most of the current ISH methods, it does multiple rounds of hybridization of the mRNA with a complementary probe which will then be fluorescence labeled and can be imaged. ([Source](https://doi.org/10.1038/nmeth.2892))  

- In each hybridization round different probes bind to the mRNA, with the sequence of images can than the sequence of the mRNA reconstructed. ([Source](https://doi.org/10.1186/s13073-022-01075-1))

- In comparison to seqFISH it uses not direct fluorescence probes but the probes contains sites for binary encoded secondary probes ([Source](https://doi.org/10.1126/science.aaa6090))


## Difference of seqFISH(A) and MERFISH(B): 

![image](https://user-images.githubusercontent.com/79060099/193455724-81d3d845-f05a-40b7-b901-3bcb5ec7c712.png)
[Image Source](https://doi.org/10.1111/febs.14435) 

## What is the benefit from MERFISH over seqFISH:

In seq-FISH with each round of hybridization the risk for an error grows exponentially for each individual target mRNA. An error in MERFISH can easier be corrected as if you encounter an unexpected sequence with the binary approach the problem is less complex than wih four different fluorphores. [More in detail](10.1126/science.aaa6090) 

## Link Technology-Application

| Technology | Statistic used (just some examples, there were many more) | Application (short term) | Application (long term) | Source |
| ----------- | ----------- | ----------- | ----------- |
| Technology | Statistic used (just some examples, there were many more) | Application (short term) | Application (long term) | Source |

| Syntax      | Description | Syntax      | Description | Source |
| ----------- | ----------- | ----------- | ----------- | ----------- |
| MERFISH (with additional retrograde labeling)      | Image analysis: deconvolution (Lucy Richardson), pixel based decoding algorithm ([similar used here](https://doi.org/10.1073/pnas.1612826113)) RNA counting: principal component analysis was used to train k nearest neighbor classier, which predicts then  a doublet score of each cell to remove cell which where to close together, normalization of RNA cell count with by the imaged volume of each cell Cell clustering: normalizing total RNA counts for each cell by the median of total RNA count of all cells. Then PCA, graph based Louvain community detection,  For presentation: UMAP | Cell atlas of primary motor cortex of a mouse     | Understanding the organization of the various cell types, which are needed to form functional neural circuits|[Source](https://doi.org/10.1038/s41586-021-03705-x)|
| MERFISH  | Processing sc-RNA-seq data: Cell ranger pipeline (10X), Seurat (normalization, batch effect removal (canonical correlation analysis, UMAP…) Segmentation: Watershed algorithm and many more Hierarchical clustering Statistical test such as: Wilcoxon rank-sum, chi square test      | Spatial organization of individual cell in fetal livers   | To better understand the hematopoeitic stem cell niche | [Source](https://doi.org/10.1038/s41421-021-00266-1) |

***
Groupmembers: EarlBugsBunny
