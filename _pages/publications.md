---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  Full list of publications on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

(\*: equal distribution)


### Published papers

- Shengen Shawn Hu, Lin Liu, Qi Li, **Wenjng Ma**, Michael J. Guertin, Clifford A. Meyer, Ke Deng, Tingting Zhang, Chongzhi Zang. Intrinsic bias estimation for improved analysis of bulk and single-cell chromatin accessibility profiles using SELMA. *Nature Communications*, (2022). [DOI](https://*doi*.org/*10.1038*/*s41467*-*022-33194*-*z*), [package](https://github.com/zang-lab/SELMA)
- **Wenjing Ma**, Sumeet Sharma, Peng Jin, Shannon L. Gourley, Zhaohui Qin. LRcell: detecting the source of differential expression at the sub-cell type level from bulk RNA-seq data. *Briefings in Bioinformatics*, (2022). [DOI](https://doi.org/10.1093/bib/bbac063), [R package](bioconductor.org/packages/release/bioc/html/LRcell.html)
  - Talk at *AWSOM workshop*, Atlanta, GA, U.S. Apr 2022. [Agenda](https://research.gatech.edu/data/events/awsom/agenda)
- **Wenjing Ma**, Kenong Su, Hao Wu. Evaluation of some aspects in supervised cell type identification for single-cell RNA-seq: classifier, feature selection, and reference construction. *Genome Biology*, (2021). [DOI](https://doi.org/10.1186/s13059-021-02480-2), [project](https://github.com/marvinquiet/RefConstruction_supervisedCelltyping)
  - Poster won **Honorable Mention** at *Georgia Statistics day*, Atlanta, GA, U.S. Oct 2021.
  - Won **Best 5-minutes presentation award** at *2nd Annual Workshop, Emerging Data Science Methods for Complex Biomedical and Cyber Data*, Augusta, GA, U.S. Oct 2021.
- **Wenjing Ma**\*, Zhenjia Wang\*, Yifan Zhang, Neal E. Magee, Yayi Feng, Ruoyao Shi, Yang Chen, Chongzhi Zang. BARTweb: a web server for transcriptional regulator association analysis. *NAR Genomics and Bioinformatics*, (2021). [DOI](https://doi.org/10.1093/nargab/lqab022), [BARTweb](http://bartweb.org/)
  - Poster at *Research in Computational Molecular Biology (RECOMB)*, Washington, D.C., U.S. May 2019.

### Collaboration papers

- Yulin Jin, Kenong Su, Ha Eun Kong, **Wenjing Ma**, Zhiqin Wang, Yujing Li, Ronghua Li, Emily Allen, Hao Wu, Peng Jin. Cell-type specific DNA methylome signatures reveal epigenetic mechanisms for neuronal diversity and neurodevelopmental disorder. *Human Molecular Genetics*, (2022). [DOI](https://doi-org.proxy.library.emory.edu/10.1093/hmg/ddac189)

### Under Review

- **Wenjing Ma**, Jiaying Lu, Hao Wu. Cellcano: supervised cell type identification for single cell ATAC-seq data. Under revision at Nature Communications, (2022). [DOI](https://doi.org/10.21203/rs.3.rs-1717357/v1), [Cellcano package](https://marvinquiet.github.io/Cellcano/)
  - Poster won [**3rd place** (out of 47)](https://franklin.uga.edu/news/stories/2022/uga-welcomed-academic-industry-partners-georgia-statistics-day) at *Georgia Statistics day*, Atlanta, GA, U.S. Oct 2022. 
  - [**2023 ASA Section on Statistics in Genomics and Genetics (SGG) Student Paper Award**](https://drive.google.com/file/d/16QTIPtHfQhACbifpEt8HCOSJCIJSYfy-/view)
  - Selected as one of four finalists to compete for the MCBIOS 2023 Young Scientist Excellence Award (YSEA) in the Student category
- Sumeet Sharma\*, **Wenjing Ma**\*, Kerry J. Ressler, Thea Anderson, Dan. C. Li, Peng Jin, Shannon L. Gourley, Zhaohui Qin. Dysregulation of prefrontal oligodendrocyte linage cells across mouse models of adversity and human major depressive disorder. Under revision, (2021).

### Posters

- BARTweb

  <img src="images/RECOMB2019_poster.png" width=300 />

- Benchmark scRNA-seq celltyping

  <img src="images/GSD2021_poster.png" width=300 />

- Cellcano

  <img src="images/GSD2022_poster.png" width=300 />