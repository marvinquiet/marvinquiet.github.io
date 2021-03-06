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

- **Wenjing Ma**, Zhenjia Wang, Yifan Zhang, Neal E. Magee, Yayi Feng, Ruoyao Shi, Yang Chen, Chongzhi Zang. BARTweb: a web server for transcriptional regulator association analysis. *NAR Genomics and Bioinformatics*, (2021). [DOI link](https://https://doi.org/10.1093/nargab/lqab022) [BARTweb link](http://bartweb.org/)

### Poster

- BARTweb: a web server for functional transcription factor prediction, *Research in Computational Molecular Biology (RECOMB)*, Washington, D.C., U.S. May 2019.

  ![RECOMB poster](/images/RECOMB2019_poster.png)

