# integrative_dp
Integrative analysis of bulk and single-cell RNA-seq datasets reveals key genes related to human hair growth and loss in dermal papilla

## Depencency
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


## Installation
1. Clone and enter this repository:
```
git clone https://github.com/Hideo-Matsuda/integrative_dp
cd integrateive_dp
```

2. Install all tools shown above.

## Differential expression analysis of bulk RNA-seq datasets.

- RNA-seq of dermal papilla (DP) cells for co-cultuered with Lactic acid bacteria (LAB) N793 strain and treated with dihydrotestosterone (DHT).

3. Run the following files using RStudio
```
01_Differential_expression_analysis_N793.Rmd
02_Differential_expression_analysis_DHT.Rmd
03_VennDiagram_of_candidate_genes.Rmd
```

Figure 2 is obtained by running "Figure2_VennDiagram_of_candidate_genes.Rmd".

## Cell-cell communication analysis of single-cell RNA-seq datasets.

- Single-cell RNA-seq for hair disease, androgenetic alopecia (AGA).


4. Obtain a preprocessed Seurat object from a repository [scScalpChromatin](https://github.com/GreenleafLab/scScalpChromatin) (Ober-Reynolds, et al., Nature Genetics, 2023).
```
git clone https://github.com/GreenleafLab/scScalpChromatin
```

Run "01_scRNA_preprocess.R" at directory ./scScalpChromatin/rna_preprocessing/
Obtain "preprocessed.rds" and copy it to directory "./rna_preprocessing/preprocessing_output_simple" in this repository.

5. Clustering and celltype identification of single-cell RNA-seq dataset. Run the following files using RStudio.
```
04_Clustering_analysis.Rmd
05_Subclustering_analysis.Rmd
06_Cell_cell_communication_analysis.Rmd
07_VennDiagram_LR.Rmd
```
Figure 3 is obtained by "Figure3_UMAP.Rmd".

6. Cell-cell communication analysis between dermal papilla cells and other cells in the dataset. Run the following file using RStudio.
```
06_Cell_cell_communication_analysis.Rmd
```

Tables 1 and 2 were obtained by this analysis.
See "06_Cell_cell_communication_analysis.html" for the result of the analysis.

7. Draw Venn diagram. Run the following file using RStudio.
```
07_VennDiagram_LR.Rmd
```

Figure 4 is obtained by "Figure4_Venn_diagram_of_genes.Rmd".

## Data

The dermal papilla sequencing data used in the paper is available in the sequence read archive (SRA) under accessions [PRJNA1089389](https://www.ncbi.nlm.nih.gov/sra/PRJNA1089389).
