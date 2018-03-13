# GO Term Enrichment using TopGO
This section describes the basic code for producing GO term enrichment analyses in R using the Bioconductor package [topGO](http://bioconductor.org/packages/release/bioc/html/topGO.html). To run TopGO, you will need:
  1.  A GO term mapping database the lists each GO term assigned to each gene
  2.  A list of reference genes
  3.  A list of test genes

First, download and install topGO in R
```R
# Download and Install topGO
source("http://bioconductor.org/biocLite.R")
biocLite()
biocLite("topGO")
library(topGO)
```

Next, we made a GO mapping file in the format:
GeneID   GO, GO, GO
This mapping file can be found here: [gene2GO](./Data/gene2GO).