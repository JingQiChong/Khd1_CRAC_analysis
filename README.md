# Khd1_CRAC_analysis

This repository focus on the analysis of CRAC data measuring the RNA-binding of yeast protein, [Khd1/Hek2](https://www.yeastgenome.org/locus/S000000128). The raw CRAC sequencing data was downloaded from the [Sequence Read Archive server (SRA)](https://www.ncbi.nlm.nih.gov/sra) and the SRA accession ID of the dataset in this repository is SRR847751. The raw CRAC sequencing data was processed and analysed by the [nf_CRACpipeline](https://github.com/JingQiChong/nf_CRACpipeline).

To run nf_CRACpipeline on Pbp2 CRAC data as in this repository, use this code and don't forget to install nf_CRACpipeline before running:

```
nextflow run ~/nf_CRACpipeline/main.nf \
--reads SRR847751.fastq \
--adapterfile input_barcodes/3primeadapter.fasta \
--novoindex input_annotation/Saccharomyces_cerevisiae.EF4.74.dna.toplevel.shortChrNames.novoindex \ 
--transcriptgff input_annotation/abundant_verified_full-ORF_ypd_plus_other_fixed_UTR_length_transcripts.gff \
--gtf input_annotation/Saccharomyces_cerevisiae.EF4.74_SGDv64_CUTandSUT_withUTRs_noEstimates_antisense_intergenic_4xlncRNAs_final.pyCheckGTFfile.output.quotefix.gtf \
--chromosome input_annotation/Saccharomyces_cerevisiae.EF4.74.dna.toplevel.shortChrNames.lengths \
--genelist input_annotation/Khd1_Ssd1TargetGeneNamesOnly.txt \
--genometab input_annotation/Saccharomyces_cerevisiae.EF4.74.dna.toplevel.shortChrNames.fa.tab \
--output_dir Khd1_SRR847751

```

# Content

The input files for the nf_CRACpipeline to process SRR847751 dataset and the analysis outputs from the pipeline are organised into subdirectories, and their contents are briefly described here. Each of the subdirectory has its own `README.md` file with more detailed description.  

## input_annotation

This subdirectory stored the annotation files (transcript maps in gff/gtf format, aligner index) required for running nf_CRACpipeline on Khd1 dataset. 

## input_barcodes

This subdirectory containes the sequencing adapters needed for running the nf_CRACpipeline on Khd1 dataset. 

## Khd1_SRR847751

The output files generated from nf_CRACpipeline are stored here.

## rmarkdown

This folder contains the rmarkdown scripts written for further analysis on SRR847751 dataset or producing figures. These scripts run after the nf_CRACpipeline has completed. 