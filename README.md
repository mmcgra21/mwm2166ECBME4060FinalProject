This repository gives the code and data needed for the paper "Gene expression analysis of patients with SARS-CoV-2 compared with other respiratory viruses" by Michael McGrath. The data can also be downloaded from the [NCBI Database](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE156063).

The repository includes the following three files, the analyses should use the files in this order:

1. `Preprocess_metadata.ipynb` - This file gives the instructions on how to download gene count data and metadata for all samples in this analysis from the [NCBI Database](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE156063). It also provides code necessary to preprocess the metadata needed for the DE and GSE analyses (see `DE_Analysis.Rmd` and `GSE_Analysis.Rmd`).

2. `DE_Analysis.Rmd` - This file runs a pairwise differential expression (DE) analysis on the gene count data and metadata downloaded and preprocessed in `Preprocess_metadata.ipynb`.

3. `GSE_Analysis.Rmd` - This file runs a gene set enrichment (GSE) analysis on the results from the pairwise DE analysis (see `DE_Analysis.Rmd`).