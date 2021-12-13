# combinatorial_treatment_analysis
This repository contains all scRNA-seq analysis data which are included in "Selective multi-kinase inhibition sensitizes mesenchymal pancreatic cancer to immune checkpoint blockade by remodeling the tumor microenvironment" by Falcomatà et al. (Nature Cancer, accepted).

FASTQ files can be found on EBIArrayExpress (https://www.ebi.ac.uk/arrayexpress/) with the dataset identifier E-MTAB-9954.
Analysis was conducted using Python (v3.8.3) and scanpy (v.1.6.0, https://github.com/theislab/scanpy).

All analysis and figures (Figures 7b, 8a, 8b, 8c; Extended data figure 9a, 9b, 9c, 9d, 10c, 10d, 10e, 10f, 10g and 10h) can be replicated by using the following jupyter notebooks:

  - Overlay_treatment_preprocessing_V02-sb.ipynb includes integration of all scRNA-seq data sets, quality control (filtering), normalization and batch correction as well as leiden clustering and initial annotation of the data set. 
  - 
