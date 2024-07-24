# LXR in Regeneration and Tumorigenesis

***
### Running the analysis

The analysis scripts for each part are available in the corresponding folder. Some datasets require manual download and should be placed in the corresponding folder. The analysis can be reproduced by installing CONDA and running the following steps:
1. Clone this repository
```
git clone https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis.git
```

2. Create and activate the conda environment based on the type of analysis you plan to run. For example, to run microarray analysis part:
```
cd LXR_in_regeneration_and_tumorigenesis
cd microarray

conda activate base
conda install -c conda-forge mamba

mamba env create -n microarray -f env_microarray.yml
conda activate microarray
```
***
### Analysis Description

The list of all analysis done in the manuscript are described below:

| Analysis | Notebook | Description | Conda Environment | Figure |
|----------|----------|-------------|-------------------|--------|
| Bulk RNAseq of Mouse Colon | [aomdss_bulk_analysis.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/AOMDSS_bulk/aomdss_bulk_analysis.Rmd) | bulk RNAseq analysis of AOM/DSS tumor kinetics in mouse colon | [aomdss_bulk_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/AOMDSS_bulk/aomdss_bulk_env.yml) | Fig. 4.c |
| Spatial Transcriptomics of Mouse Colon | [01_scRNAseq_GSE148794.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/AOMDSS_visium/01_scRNAseq_GSE148794.Rmd) | scRNAseq analysis of DSS mouse colon (GSE148794) | [aomdss_visium_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/AOMDSS_visium/aomdss_visium_env.yml) | Fig. 4.d, S10.l |
| Spatial Transcriptomics of Mouse Colon | [02_aomdss_visium_analysis.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/AOMDSS_visium/02_aomdss_visium_analysis.Rmd) | spatial transcriptomic analysis of colon tissues from standard and GW3965-diet fed mice at d22 and d43 of AOM-DSS treatment | [aomdss_visium_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/AOMDSS_visium/aomdss_visium_env.yml) | Fig. 4.d, S10.l |
| Spatial Transcriptomics of Mouse Colon | [03_aomdss_visium_deconvolution.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/AOMDSS_visium/03_aomdss_visium_deconvolution.Rmd) | cell type deconvolution using GSE148794 scRNAseq data | [aomdss_visium_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/AOMDSS_visium/aomdss_visium_env.yml) | Fig. 4.d, S10.l |
| Microarray of Human Colon | [crc_microarray_analysis.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/CRC_Microarray/crc_microarray_analysis.Rmd) | microarray analysis of human CRC samples (GSE39582) | [crc_microarray_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/CRC_Microarray/crc_microarray_env.yml) | Fig. S11.c |
| scRNAseq of Mouse Small Intestine Organoids | [organoids_sc_analysis.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Organoids_SC/organoids_sc_analysis.Rmd) | scRNAseq of mouse SI organoids treated with DMSO or GW3965 | [organoids_sc_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Organoids_SC/organoids_sc_env.yml) | Fig. S5.b-f |
| Spatial Transcriptomics of Mouse Small Intestine | [01_si_visium_analysis.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/SmallIntestine_visium/01_si_visium_analysis.Rmd) | spatial transcriptomic analysis of small intestine tissues from standard and GW3965-diet fed mice at 0- and 3-days post irradiation | [si_visium_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/SmallIntestine_visium/si_visium_env.yml) | Fig. 1.a S2.g S3.e S6.a-d |
| Spatial Transcriptomics of Mouse Small Intestine | [02_si_visium_cNMF.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/SmallIntestine_visium/02_cNMF.Rmd) | Non-negative matrix factorization analysis by cNMF package | [si_visium_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/SmallIntestine_visium/si_visium_env.yml) | Fig. 1.a S2.g S3.e S6.a-d |



***
### Datasets

The list of all datasets used in the manuscript are depicted below:

| Technology | Dataset | source publication | Accession no |
|------------|---------|--------------------|--------------|
| Spatial Transcriptomics | Irradiated Small Intestine Spatial Transcriptomics | This publication | [GSE227742](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE227742) |
| Spatial Transcriptomics | AOM/DSS Colon Visium Spatial Transcriptomics | This publication | [GSE227598](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE227598) |
| scRNAseq | Organoids scRNAseq | This publication | [GSE180079](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE180079) |
| Bulk RNAseq | AOM/DSS Colon bulk RNAseq | This publication | [GSE180078](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE180078) |
| scRNAseq | Small Intestine scRNAseq | This publication | [GSE227726](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE227726) |
| Microarray | Colon Cancer Microarray  | [Marisa et al 2013 Plos Medicine](https://journals.plos.org/plosmedicine/article?id=10.1371/journal.pmed.1001453) | [GSE39582](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE39582) |
| scRNAseq | DSS Colon scRNAseq  | [Ho et al 2021 Cell Mol Gastroenterol Hepatol](https://www.sciencedirect.com/science/article/pii/S2352345X21000758?via%3Dihub) | [GSE148794](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE148794) |
