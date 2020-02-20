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

### Publications

- **Wenjing Ma**, Zhenjia Wang, Yifan Zhang, Neal E Magee, Yang Chen and Chongzhi Zang. BARTweb: a web server for transcription factor association analysis. Feb 2020. [biorxiv](https://www.biorxiv.org/content/10.1101/2020.02.17.952838v1) [website](http://bartweb.org/)

### Poster

- BARTweb: a web server for functional transcription factor prediction, *Research in Computational Molecular Biology (RECOMB)*, Washington, D.C., U.S. May 2019.

  ![RECOMB poster](/images/RECOMB2019_poster.png)

