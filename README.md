# combinatorial_treatment_analysis
This repository contains all scRNA-seq analysis data which are included in "Selective multi-kinase inhibition sensitizes mesenchymal pancreatic cancer to immune checkpoint blockade by remodeling the tumor microenvironment" by Falcomatà et al. (Nature Cancer, accepted).

FASTQ files can be found on EBIArrayExpress (https://www.ebi.ac.uk/arrayexpress/) with the dataset identifier E-MTAB-9954.
Analysis was conducted using Python and scanpy (https://github.com/theislab/scanpy).

All analysis and figures (Figures 7b, 8a, 8b, 8c; Extended data figure 9a, 9b, 9c, 9d, 10c, 10d, 10e, 10f, 10g and 10h) can be replicated by using the following jupyter notebooks:

1) preprocessing notebooks
  - Overlay_treatment_preprocessing_V02-sb.ipynb 
  includes integration of all scRNA-seq data sets, quality control (filtering), normalization and batch correction as well as leiden clustering and initial annotation of the data set. 
  - Overlay_treatment_preprocessing_t_cells_bbknn_V01-sb.ipynb 
  includes integration of all scRNA-seq data sets and extraction of T cell clusters, quality control (filtering), normalization and batch correction as well as leiden clustering. 
  - Overlay_treatment_preprocessing_tumor_cells_bbknn_V01.ipynb 
  includes integration of all scRNA-seq data sets and extraction of Tumor cell clusters, quality control (filtering), normalization and batch correction as well as leiden clustering. 
  - Overlay_treatment_preprocessing_fibroblasts_bbknn_V01.ipynb includes integration of all scRNA-seq data sets and extraction of fibroblast clusters, quality control (filtering), normalization and batch correction as well as leiden clustering. 

2) annotation notebooks
  - Overlay_treatment_annotation_V04.ipynb annotation of the data set containing all cell types (based on leiden clustering and marker genes)
  - Overlay_treatment_t_cells_annotation_V01.ipynb annotation of the t cell data set (based on leiden clustering and marker genes)
  - Overlay_treatment_tumor_cells_annotation_V01.ipynb annotation of the tumor cell data set (based on leiden clustering and marker genes)
  - Overlay_treatment_fibroblasts_annotation_V01.ipynb annotation of the fibroblast data set (based on leiden clustering and marker genes)

3) differential expression analysis notebook
  - Overlay_treatment_tumor_cells_DGE_V01.ipynb differential gene expression analysis in tumor cells between treatment conditions

