# Khd1_CRAC_analysis

This repository focus on analysis of CRAC data measuring the RNA-binding of yeast protein, [Khd1/Hek2](https://www.yeastgenome.org/locus/S000000128). The raw CRAC sequencing data was downloaded from the [Sequence Read Archive server (SRA)](https://www.ncbi.nlm.nih.gov/sra) and the SRA accession ID is SRR847751. The raw CRAC data was processed and analysed by the [nf_CRACpipeline](https://github.com/JingQiChong/nf_CRACpipeline).

# Content

The input files for the nf_CRACpipeline and the analysis outputs from the pipeline are organised into subdirectories, and their contents are briefly mentioned here. Each of the subdirectory has its own 'README.md' file with more detailed description.  

## input_annotation

This subdirectory stored the annotation files (transcript maps in gff/gtf format, aligner index) required for running nf_CRACpipeline on Khd1 dataset. 

## input_barcodes

This subdirectory containes the sequencing adapters needed for running the nf_CRACpipeline on Khd1 dataset. 

## Khd1_SRR847751

The output files generated from nf_CRACpipeline are stored here.

## rmarkdown

This folder contains the rmarkdown scripts written for further analysis on SRR847751 dataset. These scripts run after the nf_CRACpipeline has completed. 