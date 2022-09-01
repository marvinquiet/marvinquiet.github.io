---
layout: archive
title: "Softwares"
permalink: /softwares/
author_profile: true
---

{% include base_path %}

### Python/Conda package

- [Cellcano](https://marvinquiet.github.io/Cellcano/): Cellcano is developed to do supervised cell type identification (celltyping) in scATAC-seq data. Cellcano is a two-round algorithm which utilizes confident cells predicted in the first round to predict remaining cells in the second round. [PyPI](https://pypi.org/project/Cellcano/), [conda](https://anaconda.org/marvinquiet/cellcano-all), [code](https://github.com/marvinquiet/Cellcano)

### Bioconductor package

- [LRcell](http://bioconductor.org/packages/release/bioc/html/LRcell.html) (Differential **cell** type change analysis using **L**ogitstic/linear **R**egression): LRcell is developed to identify specific (sub-)cell types that drives the changes observed in a bulk RNA-seq differential gene expression experiment. 

### Web server

- [BARTweb](https://github.com/zanglab/BARTweb_frontend)(**B**inding **A**nalysis for **R**egulation of **T**ranscription **web**): A web server hosted for performing BART analysis, which is a bioinformatics tool for predicting functional factors (including transcription factors and chromatin regulators) that bind at cis-regulatory regions to regulate gene expression in human or mouse, taking a query gene list or a ChIP-seq dataset as input.

### Research pipleines

- Explorations on strategies of constructing reference dataset for celltyping. Our paper titled "Evaluation of some aspects in supervised cell type identification for single-cell RNA-seq: classifier, feature selection, and reference construction" is accepted on *Genome Biology*. [benchmark code](https://github.com/marvinquiet/RefConstruction_supervisedCelltyping), [paper](https://doi.org/10.1186/s13059-021-02480-2)

