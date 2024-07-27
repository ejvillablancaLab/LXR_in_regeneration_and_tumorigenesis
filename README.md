# LXR in Regeneration and Tumorigenesis

***
### Running the analysis

The analysis scripts for each part are available in the corresponding folder. Some datasets require manual download and should be placed in the corresponding folder. The analysis can be reproduced by installing CONDA and running the following steps:
1. Clone this repository
```
git clone https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis.git
```

2. Create and activate the conda environment based on the type of analysis you plan to run. For example, to run microarray analysis of human colon part:
```
cd LXR_in_regeneration_and_tumorigenesis
cd Human_Colon_CRC_Microarray

conda activate base
conda install -c conda-forge mamba

mamba env create -n colon_crc_microarray_env -f colon_crc_microarray_env.yml
conda activate colon_crc_microarray_env
```
***
### Analysis Description

The list of all analysis done in the manuscript are described below:

| Analysis | Notebook | Description | Conda Environment | Figure |
|----------|----------|-------------|-------------------|--------|
| Microarray of Human Colon | [colon_crc_microarray_analysis.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Human_Colon_CRC_Microarray/colon_crc_microarray_analysis.Rmd) | microarray analysis of human CRC samples (GSE39582) | [colon_crc_microarray_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Human_Colon_CRC_Microarray/colon_crc_microarray_env.yml) | Fig. S11.c |
| Bulk RNAseq of Mouse Colon | [colon_amo-dss_bulk_analysis.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_Colon_AOM-DSS_Bulk/colon_amo-dss_bulk_analysis.Rmd) | bulk RNAseq analysis of AOM/DSS tumor kinetics in mouse colon | [colon_amo-dss_bulk_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_Colon_AOM-DSS_Bulk/colon_amo-dss_bulk_env.yml) | Fig. 4.c |
| Bulk RNAseq of Mouse Colon | [colon_dss_bulk_analysis.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_Colon_DSS_Bulk/colon_dss_bulk_analysis.Rmd) | bulk RNAseq analysis of DSS kinetics in mouse colon (GSE131032) | [colon_dss_bulk_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_Colon_DSS_Bulk/colon_dss_bulk_env.yml) | Fig. 3.c |
| Spatial Transcriptomics of Mouse Colon | [01_scRNAseq_GSE148794.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_Colon_DSS_Visium/01_scRNAseq_GSE148794.Rmd) | scRNAseq analysis of DSS mouse colon (GSE148794) | [colon_dss_visium_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_Colon_DSS_Visium/colon_dss_visium_env.yml) | Fig. 4.d, S10.l |
| Spatial Transcriptomics of Mouse Colon | [02_colon_dss_visium_analysis.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_Colon_DSS_Visium/02_colon_dss_visium_analysis.Rmd) | spatial transcriptomic analysis of colon tissues from standard and GW3965-diet fed mice at d22 and d43 of AOM-DSS treatment | [colon_dss_visium_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_Colon_DSS_Visium/colon_dss_visium_env.yml) | Fig. 4.d, S10.l |
| Spatial Transcriptomics of Mouse Colon | [03_colon_dss_visium_deconvolution.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_Colon_DSS_Visium/03_colon_dss_visium_deconvolution.Rmd) | cell type deconvolution using GSE148794 scRNAseq data | [colon_dss_visium_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_Colon_DSS_Visium/colon_dss_visium_env.yml) | Fig. 4.d, S10.l |
| scRNAseq of Mouse Small Intestine | [01_QC.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_GW_SC/01_QC.Rmd); [02_dimreduc.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_GW_SC/02_dimreduc.Rmd); [03_clustering_all.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_GW_SC/03_clustering_all.Rmd); [04_dimreduc_EPI.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_GW_SC/04_dimreduc_EPI.Rmd); [05_dimreduc_IMM_DN.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_GW_SC/05_dimreduc_IMM_DN.Rmd); [06_integration_EPI.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_GW_SC/06_integration_EPI.Rmd); [07_integration_IMM_DN.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_GW_SC/07_integration_IMM_DN.Rmd); [08_clustering_EPI.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_GW_SC/08_clustering_EPI.Rmd); [09_clustering_IMM_DN.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_GW_SC/09_clustering_IMM_DN.Rmd); [10_diffexp_EPI.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_GW_SC/10_diffexp_EPI.Rmd); [11_diffexp_IMM_DN.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_GW_SC/11_diffexp_IMM_DN.Rmd); [12_diffexp_fullsamples.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_GW_SC/12_diffexp_fullsamples.Rmd); | scRNAseq analysis of small intestine tissues from standard and GW3965-diet fed mice for 10 days | [si_gw_sc_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_GW_SC/si_gw_sc_env.yml) | Fig. S2.a-f, h-i |
| scRNAseq of Mouse Small Intestine | [si_irrad_sc_analysis.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_Irrad_SC/si_irrad_sc_analysis.Rmd) | scRNAseq analysis of small intestine crypts from mice at 0- and 3-days post irradiation (GSE117783) | [si_irrad_sc_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_Irrad_SC/si_irrad_sc_env.yml) | Fig. 3.b |
| Spatial Transcriptomics of Mouse Small Intestine | [01_si_irrad_visium_analysis.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_Irrad_Visium/01_si_irrad_visium_analysis.Rmd) | spatial transcriptomic analysis of small intestine tissues from standard and GW3965-diet fed mice at 0- and 3-days post irradiation | [si_irrad_visium_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_Irrad_Visium/si_irrad_visium_env.yml) | Fig. 1.a, S2.g, S3.e, S6.a-d |
| Spatial Transcriptomics of Mouse Small Intestine | [02_cNMF.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_Irrad_Visium/02_cNMF.Rmd) | Non-negative matrix factorization analysis by cNMF package | [si_irrad_visium_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_Irrad_Visium/si_irrad_visium_env.yml) | Fig. 1.a, S2.g, S3.e, S6.a-d |
| scRNAseq of Mouse Small Intestine Organoids | [si_organoids_gw_sc_analysis.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_Organoids_GW_SC/si_organoids_gw_sc_analysis.Rmd) | scRNAseq of mouse small intestine organoids treated with DMSO or GW3965 | [si_organoids_gw_sc_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Mouse_SI_Organoids_GW_SC/si_organoids_gw_sc_env.yml) | Fig. S5.b-f |
| Regeneration Associated DEGs | [Reg_DEGs_KEGG_analysis.Rmd](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Regeneration_Associated_DEGs/Reg_DEGs_KEGG_analysis.Rmd) | DEG overlap between regenerative and steady state colonic tissue and small intestine crypts following DSS-induced colitis and irradiation plus KEGG pathway analysis  | [Reg_DEGs_KEGG_env.yml](https://github.com/ejvillablancaLab/LXR_in_regeneration_and_tumorigenesis/blob/main/Regeneration_Associated_DEGs/Reg_DEGs_KEGG_env.yml) | Fig. S1.a |

***
### Datasets

The list of all datasets used in the manuscript are depicted below:

| Technology | Dataset | Source Publication | Accession no |
|------------|---------|--------------------|--------------|
| Microarray | Human Colon Cancer Microarray | [Marisa et al 2013 Plos Medicine](https://journals.plos.org/plosmedicine/article?id=10.1371/journal.pmed.1001453) | [GSE39582]
| Bulk RNAseq | Mouse AOM/DSS Colon bulk RNAseq | This publication | [GSE180078](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE180078) |
| Spatial Transcriptomics | Mouse Irradiated Small Intestine Visium Spatial Transcriptomics | This publication | [GSE227742](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE227742) |
| Spatial Transcriptomics | Mouse AOM/DSS Colon Visium Spatial Transcriptomics | This publication | [GSE227598](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE227598) |
| scRNAseq | Mouse Small Intestine Organoids scRNAseq | This publication | [GSE180079](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE180079) |
| scRNAseq | Mouse Small Intestine scRNAseq | This publication | [GSE227726](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE227726) |
(https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE39582) |
| scRNAseq | Mouse DSS Colon scRNAseq | [Ho et al 2021 Cell Mol Gastroenterol Hepatol](https://www.sciencedirect.com/science/article/pii/S2352345X21000758?via%3Dihub) | [GSE148794](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE148794) |
| scRNAseq | Mouse Irradiated Colon scRNAseq | [Ayyaz et al 2019 Nature](https://www.nature.com/articles/s41586-019-1154-y) | [GSE117783](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE117783)
| Bulk RNAseq | Mouse DSS Colon Bulk RNAseq | [Czarnewski et al 2019 Nat Commun](https://www.nature.com/articles/s41467-019-10769-x) | [GSE131032](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE131032) |
