This repo contains R scripts to perform scRNAseq data analysis followed by cellular interaction analysis using cellphoneDB.
This work is part of a manuscript titled "Enhanced NK cell proficiency in solid tumors through antigen-specific memory via NKG2C/A-HLA-E/ABC recruited to tumors by CXCR2"

Dataset ID - GSE184880 

scRNAseq_analysis.Rmd - 
The file includes R code to perform scRNAseq clustering and analysis as depicted in Figures 2 A-C of the manuscript. 
Raw gene counts were downloaded from GEO and analysed using the Seurat package (version 4.4.0). NK and myeloid clusters were identified from the overall clustering involving all cells using this script. NK and myeloid clusters were further subclustered and annotated using a similar pipeline.

cellphonedb.Rmd - 
This file includes R code to run cellphoneDB (Efremova, M. et al., Nat Protoc, 2020) as depicted in Figures 2 D-F of the manuscript. CellphoneDB was employed to compute interactions between myeloid and NK clusters by utilizing its database of known ligand-receptor interactions. 
