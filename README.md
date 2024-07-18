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
### Datasets

The list of all datasets used in the manuscript are depicted below:

| Technology | Dataset | source publication | Accession no |
|------------|---------|--------------------|--------------|
| Microarray | Colon Cancer Microarray  | [Marisa et al 2013  Plos Medicine]( https://journals.plos.org/plosmedicine/article?id=10.1371/journal.pmed.1001453)| [GSE39582]( https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE39582) |
