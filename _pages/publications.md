---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}


### Published

- **Wenjing Ma**, Sumeet Sharma, Peng Jin, Shannon L. Gourley, Zhaohui Qin. LRcell: detecting the source of differential expression at the sub-cell type level from bulk RNA-seq data. Accepted by *Briefings in Bioinformatics*, (2022). [R package](bioconductor.org/packages/release/bioc/html/LRcell.html), [DOI](https://doi.org/10.1093/bib/bbac063).
- **Wenjing Ma**, Kenong Su, Hao Wu. Evaluation of some aspects in supervised cell type identification for single-cell RNA-seq: classifier, feature selection, and reference construction. *Genome Biology*, (2021). [DOI](https://doi.org/10.1186/s13059-021-02480-2), [project](https://github.com/marvinquiet/RefConstruction_supervisedCelltyping)
- **Wenjing Ma**\*, Zhenjia Wang\*, Yifan Zhang, Neal E. Magee, Yayi Feng, Ruoyao Shi, Yang Chen, Chongzhi Zang. BARTweb: a web server for transcriptional regulator association analysis. *NAR Genomics and Bioinformatics*, (2021). [DOI](https://doi.org/10.1093/nargab/lqab022), [BARTweb](http://bartweb.org/)

### Under Review

- Yulin Jin, Kenong Su, Ha Eun Kong, **Wenjing Ma**, Zhiqin Wang, Yujing Li, Ronghua Li, Emily Allen, Hao Wu, Peng Jin. Cell-type specific DNA methylome signatures reveal epigenetic mechanisms for neuronal diversity and neurodevelopmental disorder. Under review, (2022).
- Sumeet Sharma\*, **Wenjing Ma**\*, Kerry J. Ressler, Thea Anderson, Dan. C. Li, Peng Jin, Shannon L. Gourley, Zhaohui Qin. Dysregulation of prefrontal oligodendrocyte linage cells across mouse models of adversity and human major depressive disorder. Under review, (2021).
- Shengen Shawn Hu, Lin Liu, Qi Li, **Wenjng Ma**, Michael J. Guertin, Clifford A. Meyer, Ke Deng, Tingting Zhang, Chongzhi Zang. Accurate estimation of intrinsic biases for improved analysis of chromatin accessibility sequencing data using SELMA. Under review, (2021). [bioRxiv](https://www.biorxiv.org/content/10.1101/2021.10.22.465530v1)


## Poster

- **Honorable Mention**. Evaluation of some aspects in supervised cell type identification for single-cell RNA-seq, *Georgia Statistics day*, Atlanta, GA, U.S. Oct 2021.
  
  <img src="/images/GSD2021_poster.png" width=300 />

- BARTweb: a web server for functional transcription factor prediction, *Research in Computational Molecular Biology (RECOMB)*, Washington, D.C., U.S. May 2019.

  <img src="/images/RECOMB2019_poster.png" width=300 />


## Talk

- **Best 5-minutes presentation award**. Evaluation of some aspects in supervised cell type identification for single-cell RNA-seq, *2nd Annual Workshop, Emerging Data Science Methods for Complex Biomedical and Cyber Data*, Augusta, GA, U.S. Oct 2021.
