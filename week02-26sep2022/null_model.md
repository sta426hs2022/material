# Bubble-Seq
## How does it works?
- During the cell devision in the S-Phase originis of replcation determine the replication start site.   
- The bubble is formed around theses sites. 
- Due to the circular nature of the fragments containing these bubbles, they can be identified using agarose gel seperation.
## Aplication
- Determination of genomwide origin maps
## What statistics is used afterwards?
### Preparation:
#### Establish significant levels for library fragments
- Calculate a robust estimate of the read depth: number of reads in each EcoRI fragment/ fragment length in base pairs
- Fit the low end of the read depth distribution (background or noise) to a negative binomial distribution -> calculate P-values and false discovery rates (FDRs) for every EcoRI fragment in the genome.
- Define bona fide bubble-containing fragments at a false discovery rate of 0.1\% (“bona fide” means in good faith)
#### Apply filters to remove artifacts such as EcoRI fragments <500 bp, exclude larger fragments containing ≥ 80\% alpha-satellite, make pairwise comparisons among the three data sets
### The model itself:
#### discrete distribution of the null model $p^2 *(1- p)^n$
- p = probability of finding a bubble-containing fragment in the genome
- n = number of negative fragments between two bubble-containing fragments
- assume that the probability of an EcoRI fragment containing a bubble or not containing a bubble is independent of the bubble-containing status of its neighbors.
- estimate the probability p of a genomic EcoRI fragment containing a bubble: fraction of EcoRI fragments containing bubbles
- using above assumptions, the probability of finding two bubble-containing fragments separated by n non-bubble-containing fragments is given by $p^2 *(1- p)^n$.

By Himmelgrau, msalzm, georgeastakhov2
