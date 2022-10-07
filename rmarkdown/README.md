# rmarkdown
This directory contain rmarkdown script for Khd1 CRAC analysis. These are run after the nf_CRACpipeline has completed.

## peakanalysis_khd1.Rmd 
This script searches for motifs associated with Khd1-bound RNA from the CRAC datasets

## pileup_Khd1_closeup.Rmd 
This script generates plot for the pileup analysis result of Khd1 CRAC datasets

## pileup_Khd1_targetgenes.Rmd
This script selects a list of potential genes that might be regulated by Khd1 and generate text file that will be use in pileup analysis.

## Bedgraph_Ssd1_Khd1_plots.Rmd
This script produces genome browser-style figures of Khd1 CRAC profiles from bedgraph data. 

## peakanalysis_crosslinkedsites_khd1.Rmd
This script extracts sequences near the Khd1 cross-linked peaks (+/-25 bases) and put them into a fasta file.
