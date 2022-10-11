# DUP-SEQ (Duplex sequencing)
> Github.usernames: JulianKlinkmann DonJuliano, AsraAbukar

## Short summary
Duplex sequencing is an error corrected NGS technology in which technical errors that occur in the amplification phase are significantly reduced by labelling both complementary DNA strands. This technology is used for multiple application purposes, and depending on the application the suitable statistical model is used for the analysis of the data. 

Technology  | Application | Statistic
------------- | -------------|----------
Dup-seq  | determination mutation frequency of mutagens | Generalized linear mixed model (GLMM) 
 || determination of rare mutation | binomial model


## Technology

Usually, Sequencing technologies have an error rate of roughly 1%. Duplex Sequencing provides a viable solution to this problem 
and provides an upgrade to the classical Illumina high throughput sequencing. 

A double strand of DNA gets tagged. The tags, in combination with differing arms, enable 5 - 3 and 3 - 5 identification after sequencing.


When we have multiple strands, they get sequenced like in usual Illumina. As a result, we yield multiple copies of the same strand. 

Only, if a mutation is detected in every strand (green), it is considered a mutation. Other seeming mutations (pink, yellow) are due to PCR-mistakes. 

![Dup-Seq](https://www.pnas.org/cms/10.1073/pnas.1208715109/asset/b789bfa6-b7db-4840-9d39-71b822433de4/assets/graphic/pnas.1208715109fig01.jpeg)


## Application

As high throughput sequencing comes with a lot of noise, it is very hard to identify allele variants with low frequencies (under 1%).
Therefore, Dup-seq is useful for every application, which requires to detect low-frequency mutations. 

In humans, there are numerous disease-causing mitochondrial variants. For mitochondrial replacement therapies like tri-parental in vitro fertilization, which can prohibit mitochondrial-caused diseases, stable identification of rare variants is vital. 

Same accounts for early detection of carcinogenesis, which also relies on detecting and characterizing mutagenesis. 


## Statistical methods

[In Source 4](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7776782/), a χ2 test was carried out to compare the base substitution spectra detected in a gene by Duplex sequencing and transgenic rodent assay.
Generaluzed linear mixed model (GLMM) with binomial error distribution are used to get the estimated mutation frequancy.<sup>[5](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-022-08752-w)</sup> 
For the determination of rare mutation the Wilson score interval method (binomial model) was used. <sup>[1](https://www.pnas.org/doi/full/10.1073/pnas.1208715109)</sup>





[Source 1](https://www.pnas.org/doi/full/10.1073/pnas.1208715109)

[Source 2](https://link.springer.com/content/pdf/10.1186/s13059-016-1039-4.pdf)

[Source 3](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5714827/)

[Source 4](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7776782/)

[Source 5](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-022-08752-w)
