# Introduction-to-metagenomics-analysis
BI practicum 7

This lab report demonstrates the study of a history of oral diseases in humans.

Scientists extracted DNA from the material underneath the dental calculus of a microbial community that was buried by layers of dental calculus and was kept intact for more than 1000 years. We will be using samples from dental calculus, and will compare them with the samples from the ancient tooth roots.

This repository contains a jupyter notebook where the workflow is described and a .pdf file with the lab report. It also contains an .Rmd file with alternative 16S analisys with DADA2.

## Data

This lab work uses the following data:
- original [study](https://trace.ncbi.nlm.nih.gov/Traces/sra/?study=SRP029257)
- a pre-trained [Naive Bayess classifier](https://data.qiime2.org/2022.2/common/silva-138-99-nb-classifier.qza)
- shotgun sequencing [data](https://www.ncbi.nlm.nih.gov/sra/SRX340014[accn])
- T. forsythia strain [reference genome](https://www.ncbi.nlm.nih.gov/nuccore/NC_016610.1)

## Key results

The annotation of crossed regions showed a fair amount of transposase coding genes. Transposase genes encode enzymes responsible for the movement of transposable elements within the genome, contributing to genome plasticity, evolution, and adaptation.

## Usage

To reproduce the enviroment use:
```bash
conda env create -f environment.yml
conda activate qiime2-amplicon-2024.2
```

It is possible that this enviroment won't be built, if so ~~very sad~~ use the [guide](https://docs.qiime2.org/2024.2/install/native/) to install qiime2 and then manually install all other dependencies. 
