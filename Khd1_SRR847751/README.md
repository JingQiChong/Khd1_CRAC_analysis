# Khd1_SRR847751

This directory contains selected output of the nf_CRACpipeline running on the Khd1 SRR847751 dataset. Files exceeding the file size limit of GitHub (100Mb) such as trimmed fastq and aligned sam file are not included in this directory.  

## aligned_bamqc

File containing the BamQC analysis result that shows the quality of read alignments.

## aligned_bamsorted

Sorted bam files and their respective index file. Generated from samtools.

## bedgraph_files

bedgraph files (separated for minus and plus strand reads) showing counts of (deduplicated) aligned reads on the whole genome. Generated from the gtf files that were produced by pyReadcounter.py 

## bedgraph_genomecov

bedgraph files (separated for minus and plus strand reads) showing counts of aligned reads on the whole genome. Generated from the sorted indexed bam files using bedtools genomecov

## collapsed

Fasta file that stored the demulitplexed and deduplicated reads.

## demultiplexed_fastqc

FastQC analysis result on the demultiplexed and deduplicated reads.

## MEME

Files generated by the MEME software that performed motif analysis using the output files from the nf_CRACpipeline.

## multicov_analyses

Tab-separated gff-like text file containing the number of reads overlapped with annotated transcripts. Generated by multiBamCov.

## pyCalculateFDRs_analyses

Tab-separated gtf-like text files showing the location, heights, and false discovery rate (FDR) of each peaks on protein-coding genes. Generated by pyCalculateFDR.py.

## pyPileup_analyses

Tab-separated text files showing the read counts, deletion and substitution data for each base of the selected Khd1 target transcripts.

## pyReadCounters_analyses

Analysis result by pyReadCounters.py demonstrating the number of CRAC reads that were overlapped to the genomic features of target organisms. Statistics and log of the analysis are in included this folder as well. 

## pyReadCountersBlocksNoMuts_analyses

Same analysis by pyReadCounters.py but no mutations were reported.
