# Characterisation of Natural Transformation in Chromobacteriaceae
## Master’s Thesis Code Repository
This repository contains the code developed and used in my master’s thesis investigating natural transformation in the Chromobacteriaceae family. The project integrates bioinformatic analyses to identify DNA uptake sequence (DUS)-like motifs, assess their genomic distribution, and explore the genetic context of competence-related genes.
The purpose of this repository is to ensure transparency, reproducibility, and accessibility of all computational analyses performed during the study.

### Project Overview

Natural transformation is a key mechanism of horizontal gene transfer (HGT), well characterised in Neisseriaceae but largely unexplored in environmental relatives such as Chromobacteriaceae.

This repository supports analyses aimed at:
- Identifying overrepresented sequence motifs (putative ChromoDUS)
- Quantifying motif density across genomes
- Assessing enrichment relative to background nucleotide composition
- Visualising motif distribution patterns
- Mapping gene neighbourhoods of competence-associated gene comP
- Modelling ComP of genus-representatives from Chromobacteriacea using AlphaFold

### Repository Structure

Each file in `script` corresponds to a specific methodological section in the thesis.  

#### 3.1.2 – Search for overrepresented sequences
- `r-finder` --> Tool used to identify candidate overrepresented motifs across genomes
- `Sequence_logos.rmd` --> Generates sequence logos to visualise motif conservation

#### 3.1.3 – Identification and quantification of DUS density
- `Heatmap_DUS.rmd` --> Calculates DUS frequency (DUS/Mb) across genomes and visualises distributions

#### 3.1.4 – Comparative heatmap construction and data visualisation
- `Heatmap_DUS.rmd` (Shared with Section 3.1.3)
- `Overexpression_Heatmap.rmd` --> Computes enrichment ratios (observed vs expected) and generates comparative heatmaps

#### 3.1.6 – Construction of gene neighbourhood maps
- `United_GeneMap.rmd` Generates operon/gene neighbourhood visualisations for comP and associated genes

Additionally in the `results` folder one can find results from r-finder, OperonMapper, AlphaFold and the images produced from the scripts. 

### Requirements
The analyses were primarily conducted in R. Required packages are listed in the `grateful-report.html`
Note: Some scripts may require additional dependencies depending on your environment.

### Data
Genomic data used in this project were obtained from publicly available databases (e.g., NCBI RefSeq).
Due to file size and licensing considerations, raw genome files are not included in this repository.

### Reproducibility Notes

File paths in scripts may need to be adapted to your local environment.
Some analyses depend on external tools (e.g., motif discovery pipelines).
Parameter choices reflect the scope and level of a master’s thesis and may be simplified compared to full-scale bioinformatic pipelines. 

#### Author
Oliwia Hillestad Waz
Master’s Thesis in Biomedicine at OsloMet 

#### Acknowledgements

This work was conducted as part of a master’s thesis project. I acknowledge main supervisors Ole Herman Ambur and collaborators Kristian Alfsnes, Stephan A. Frye, Alexander Hesselberg Løvestad, and, Stian Aleksander Helsem for guidance in both experimental design and computational analysis.

#### License
This repository is shared for academic and educational purposes.
Please cite appropriately if you reuse code or concepts from this work.



