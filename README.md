# integrative_dp
Integrative analysis of bulk and single-cell RNA-seq datasets reveals key genes related to human hair growth and loss in dermal papilla

# Depencency
- R (tested with version 4.3.1)
- RStudio (tested with version 2023.03.0-386)
- TCC (tested with version 1.38.0)
- VennDiagram (tested with version 1.7.3)
- Matrix (tested with 1.5-1)
- dplyr (tested with 1.1.2)
- Seurat (tested with 4.3.0.1)
- patchwork (tested with 1.1.3)
- future (tested with 1.33.0)
- stringr (tested with 1.5.0)
- TxDb.Hsapiens.UCSC.hg38.knownGene (tested with 3.17.0)
- org.Hs.eg.db (tested with 3.17.0)
- tidyverse (tested with 2.0.0)
- magrittr (tested with 2.0.3)
- liana (tested with 0.1.13)


# Installarion
1. Clone and enter this repository:
```
git clone https://github.com/Hideo-Matsuda/integrative_dp
cd integrateive_dp
```

2. Install all tools shown above.

<<<<<<< HEAD
# Differential expression analysis of bulk RNA-seq datasets.

- RNA-seq of dermal papilla (DP) cells for co-cultuered with Lactic acid bacteria (LAB) N793 strain and treated with dihydrotestosterone (DHT).

=======
# Differential expression analysis of RNA-seq datasets of dermal papilla cells for co-cultuered with Lactic acid bacteria N793 strain and treated with dihydrotestosterone (DHT).
>>>>>>> origin/main
3. Run the following files using RStudio
```
01_Differential_expression_analysis_N793.Rmd
02_Differential_expression_analysis_DHT.Rmd
03_VennDiagram_DEGs.Rmd
```

Figures 2 (a) and (b) were obtained by this analysis.
See "03_VennDiagram_DEGs.html" for the result of the analysis.

<<<<<<< HEAD
# Cell-cell communication analysis of single-cell RNA-seq datasets.

- Single-cell RNA-seq for hair disease, androgenetic alopecia (AGA).

4. Clustering and celltype identification of single-cell RNA-seq dataset. Run the following files using RStudio
=======
# Cell-cell communication analysis of single-cell RNA-seq datasets for hair disease, androgenetic alopecia (AGA),
4. Obtain a preprocessed Seurat object from a repository (Ober-Reynolds, et al., Nature Genetics, 2023),
```
git clone https://github.com/GreenleafLab/scScalpChromatin
```

Run "01_scRNA_preprocess.R" at directory ./scScalpChromatin/rna_preprocessing/
Obtain "preprocessed.rds" and copy it to directory "integrative_dp/rna_preprocessing/preprocessing_output_simple" in this repository.

5. Clustering and celltype identification of single-cell RNA-seq dataset. Run the following files using RStudio
>>>>>>> origin/main
```
04_Clustering_analysis.Rmd
05_Subclustering_analysis.Rmd
06_Cell_cell_communication_analysis.Rmd
07_VennDiagram_LR.Rmd
```

Figure 3 (a), (b), and (c) were obtained by this analysis.
See "04_Clustering_analysis.html", "05_Subclustering_analysis.html" for the result of the analysis.

<<<<<<< HEAD
5. Cell-cell communication analysis between dermal papilla cells and other cells in the dataset. Run the following file using RStudio
=======
6. Cell-cell communication analysis between dermal papilla cells and other cells in the dataset. Run the following file using RStudio
>>>>>>> origin/main

```
06_Cell_cell_communication_analysis.Rmd
```

Tables 1 and 2 were obtained by this analysis.
See "06_Cell_cell_communication_analysis.html" for the result of the analysis.

<<<<<<< HEAD
6. Draw Venn diagram. Run the following file using RStudio
=======
7. Draw Venn diagram. Run the following file using RStudio
>>>>>>> origin/main

```
07_VennDiagram_LR.Rmd
```

Figure 4 (a) and (b) were obtained by this analysis.
See "07_VennDiagram_LR.html" for the result of the analysis.

# Data

The dermal papilla sequencing data used in the paper is available in the sequence read archive (SRA) under accessions [PRJNA1089389](https://www.ncbi.nlm.nih.gov/sra/PRJNA1089389).
