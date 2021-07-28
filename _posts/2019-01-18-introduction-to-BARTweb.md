```
---
title: "Introduction to BARTweb"
collection: talks
type: "Lab Meeting"
permalink: /talks/2019-01-18-introduction-to-BARTweb
venue: "Joint lab meeting at Center for Public Health Genomics, University of Virginia"
date: 2019-01-18
location: "Charlottesville, Virginia"
---
```

[Slides here] (https://www.dropbox.com/s/7o7duis8ftzz9yi/BARTweb_Wenjing_2018.01.18.pptx?dl=0)

### Why BART?

- BART can be used to analyze Differentially Expressed Genes (DEG)

  Traditional ways of doing downstream analysis on a bunch of differentially expressed genes are Gene Ontology analysis such as [DAVID](https://david.ncifcrf.gov/), or Pathway analysis such as [KEGG](https://www.genome.jp/kegg/). Both methods **lack information in which TFs regulate the genes**.

- Conventional TF prediction methods are sequence-based

  The most popular method of TF prediction is to scan motifs, which only values the promoter regions near the Transcription Start Site (TSS). In other word, it left out distal enhancers. Meanwhile, a sequence-based method engenders a problem that multiple factors may share similar motifs, increasing the chance of finding a wrong TF. Furthermore, a motif does not necessarily mean a binding.

That is what BART can do - to predict functional regulatory TFs when given a gene list or a ChIP-seq genomic binding profile.

### BART workflow



### Why BARTweb?

From the workflow, you probably notice that both MARGE and BART leverage a large amount of data, which occupy tremendous disk space and bring intensive computation load. With the growth of H3K27ac and TF ChIP-seq public data size, the problem is getting worse. 

To release the burden of biomedical researchers, we consider developing this web interface, named [BARTweb](http://bartweb.org), to run users' jobs on our computing cluster. For now, we are working on updating the H3K27ac and TF ChIP-seq dataset, in the meantime, optimizing the algorithm to shorten the job execution time. Our new version can help reduce job running time from 1.5 hours to 5-10 mins and will be released soon!

For your reference, the table below indicates the data amount we involve in our current version versus our next version.

|              | H3K27ac samples | TF ChIP-seq dataset | TF counts |    UDHS(UAC)    |
| :----------: | :-------------: | :-----------------: | :-------: | :-------------: |
| BARTweb V1.1 |     366/267     |      7032/5023      |  883/531  | 2732010/1529448 |
| BARTweb V1.2 |    1230/737     |      7987/5887      | 1300/700  | 4157285/2687740 |

For more details behind BARTweb, please refer to the slides by this [link](https://www.dropbox.com/s/7o7duis8ftzz9yi/BARTweb_Wenjing_2018.01.18.pptx?dl=0).
