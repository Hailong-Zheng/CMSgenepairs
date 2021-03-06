# CMSgenepairs
CMSgenepairs is a gene pair-based classifier to classfy the Consensus Molecular Subtypes (CMS) of colorectal cancer. The CMSgenepairs can  identify stable CMS labels for the given samples and be well applied to the single sample data.

# Install
To install the CMSgenepairs, install from github using devtools
```
install.packages(randomForest)
library(devtools)
install_github("Hailong-Zheng/CMSgenepairs")
```
Or you can download the .ZIP file and and unzip it.
```
install.packages("CMSgenepairs",repos = NULL,type="source")
#The "CMSgenepairs" should be combined with the absolute path.
```
# Usage
```
library(CMSgenepairs)
data(example)
CMS_label=CMSgenepairs(Exp)$predictedCMS
```
The example is the gene expression profile of GSE31595 from database Gene Expression Omnibus (GEO)
# Data input
Exp, a dataframe with gene expression profiles data values, samples in columns, genes in rows, rownames corresponding to Entrez IDs. 
The CMSgenepairs can be well applied to Affymetrix Array data (Series Matrix File) and RNA-seq data (RPKM). 

# Contact email
Please don't hesitate to address comments/questions/suggestions regarding this R package to:
zhaowenyuan@ems.hrbmu.edu.cn
