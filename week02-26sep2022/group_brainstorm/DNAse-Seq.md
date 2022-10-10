# DNAse-Seq

> team: GretaBordinETH, Jieran-S, Mayiiiiii, Richta-Kumar

Analysis of chromatin states and positioning of regulatory proteins.

## Mechanism
1. Cells are lysed to release nuclei which are digested with DNase I, DNA sequences bound by regulatory proteins are protected from DNase l digestion;
2. DNase I digested DNA fragments are blunt-ended, extracted and ligated;
3. The DNA fragments are amplified by PCR and sequenced with a deep sequencing method of choice (most often, Illumina).

From the obtained reads it is possible to identify DNA clips where the regulatory proteins of interest were located.

| ![Mechanism sequecing](https://emea.illumina.com/content/dam/illumina-marketing/images/tools/sequencing/dnase-seq-dnasel-seq.png)
|:--:|
| <b> Sequencing mechanism for DNAse Sequencing. Retreived from https://emea.illumina.com/science/sequencing-method-explorer/kits-and-arrays/dnase-seq-dnasel-seq.html</b>|

## Statistical Methods for analysis

* One common model to identify protein-binding footprints from digital footprinting data using DNAse sequencing is the **dynamic Bayesian network**. It detects candidate footprints as regions of depleted cleavage relative to a local background and assigns a statistical confidence estimate to each candidate based on an empirical null model. 
* Another common statistical model incorporates DNase-seq data and PWMs within a **multivariate hidden Markov model** (HMM) to detect footprint-like regions with matching motifs
* Kernel density estimation

## Applications

* DNAse sequencing is a highly efficient tool to detect the active gene regulatory elements that governs various biological processes, specially for DNase 
hypersensitive (HS) sites. 
* Comparing to the traditional way of Southern blot, the method is more efficienty by capturing DNase-digested fragments and high-throughput sequencing. 

## Further reading

* https://academic.oup.com/bioinformatics/article/26/12/i334/281986
* https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3627383/
* https://emea.illumina.com/science/sequencing-method-explorer/kits-and-arrays/dnase-seq-dnasel-seq.html
* https://www.frontiersin.org/articles/10.3389/fgene.2012.00230/full
