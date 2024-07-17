# MESO_2025


# Intra-tumoral T cells in pediatric brain tumors display clonal expansion and effector properties
------------

Description
------------

Mesothelioma is a cancer....

Requirements
------------

This project was done using the following modules/programs:

* [R](https://cran.r-project.org/) (v)
* [Cell Ranger](https://support.10xgenomics.com/single-cell-gene-expression/software/pipelines/latest/what-is-cell-ranger) (v3.1.0)
* [Scrublet](https://github.com/swolock/scrublet/blob/master/README.md) (v0.2.3)
* [Seurat](https://satijalab.org/seurat) (v)
* [vdjtools](https://vdjtools-doc.readthedocs.io/en/master/) (v1.2.1)

Raw data
------------
* The single-cell RNA-seq raw and processed files from PBT and NSCLC (our study) can be downloaded through the following GEO accession number: []() 



Raw data pre-processing  
------------

### Single-cell
* To do the 10x demultiplexing and mapping pull [our in-house pipeline](https://github.com/vijaybioinfo/cellranger_wrappeR) using Cell Ranger.
* To do the donor demultiplexing pull [our in-house pipeline](https://github.com/vijaybioinfo/ab_capture).
* To do the single-cell quality control pull [our in-house pipeline](https://github.com/vijaybioinfo/quality_control).
* To do the doublet detection use [our in-house pipeline](https://github.com/vijaybioinfo/doublet_detection) using Scrublet. 
* To generate the clustering of single-cell data just pull [our in-house pipeline](https://github.com/vijaybioinfo/clustering) using Seurat.
* To do the aggregation of VDJ libraries pull [our in-house pipeline](https://github.com/vijaybioinfo/VDJ_aggr).  

> Relevant scripts are located in: ./pre-processing  

For more specific information about the data generation and processing, please check the "methods" section within the manuscript.  

### Bulk   
Patients diagnosed with High-Grade Gliomas (HGG; n=120) with records of age (<20 years old) and sex were considered for the survival analysis. RNA-seq samples of the donors classified as metastasis or with unavailable TUMOR TYPE information were filtered out; samples derived from cell lines or obtained from the spine region were also excluded. The final list of donor samples can be found in: ./pre-processing 


Figures
------------
> Relevant scripts are located in: ./figures


Downstream Analysis
------------
* DGEA - You can follow [our in-house pipeline](https://github.com/vijaybioinfo/dgea)
* [GLIPH2](http://50.255.35.37:8080/) - Clustering of CDR3β sequences
* [vdjtools](https://vdjtools-doc.readthedocs.io/en/master/) - TCR diversity estimation
> Relevant scripts all located in: ./downstream_analysis


Usage & Citation
--------------

If you want to clone this repository run:
```bash
git clone https://github.com/vijaybioinfo/MESO_2025.git
```
Please cite the following manuscript if you are using this repository:  


Maintainers
-----------

Current maintainers:
* Kevin Meza Landeros (kmlanderos@lji.org) 

Vijayanand Lab.  
Division of Vaccine Discovery La Jolla Institute for Immunology La Jolla, CA 92037, USA


Contact
-----------
Please email Kevin Meza Landeros (kmlanderos@lji.org) and/or Vijayanand Pandurangan (vijay@lji.org).
