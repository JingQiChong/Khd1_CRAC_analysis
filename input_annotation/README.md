# input_annotation

This directory contains genome sequences, annotations, aligner index and gene lists used to process and analyse Khd1 CRAC data.

## abundant_verified_full-ORF_ypd_plus_other_fixed_UTR_length_transcripts.gff

gff format file containing the end to end location of messenger RNA transcripts. For more details, please refer to [Ssd1_CRACanalysis_2020 repository](https://github.com/ewallace/Ssd1_CRACanalysis_2020/tree/master/input_annotation).

## gff_ncRNAs_abundantverifiedmRNAparts.gff

Transcript annotations with non-coding RNAs, and mRNAs broken down into parts (5′UTR,CDS, intron, 3′UTR). For more details, see [Ssd1_CRACanalysis_2020 repository](https://github.com/ewallace/Ssd1_CRACanalysis_2020/tree/master/input_annotation).

## Khd1_TargetGeneNameOnly.txt

The names of select Khd1 target genes, that are used as input for detailed pileup maps in `pyPileup.py` of the nf_CRACpipeline.

## Saccharomyces_cerevisiae.EF4.74_SGDv64_CUTandSUT_withUTRs_noEstimates_antisense_intergenic_4xlncRNAs_final.pyCheckGTFfile.output.quotefix.gtf

Transcript map in gtf file format that includes mRNA annotations from EF4.74, and many classes of ncRNA including unstable transcripts (CUTs, SUTs). This file is from David Tollervey's lab. 

## Saccharomyces_cerevisiae.EF4.74.dna.toplevel.shortChrNames.fa

*Saccharomyces cerevisiae* genome sequence in .fasta format from ensemble release EF4.74, which is identical to SGD release R64-1-1. The chromosome names was edited to be `chrI, chrII, ...`.

Index file for this fasta,  `Saccharomyces_cerevisiae.EF4.74.dna.toplevel.shortChrNames.fa.fai` is not included in the repository as the index file can be made fresh locally by script in this repository.

## Saccharomyces_cerevisiae.EF4.74.dna.toplevel.shortChrNames.fa.tab

Tab-separated variable format file that has the same data as `Saccharomyces_cerevisiae.EF4.74.dna.toplevel.shortChrNames.fa`. This file is required by some of the pyCRAC suite tools that are included in the nf_CRACpipeline.

## Saccharomyces_cerevisiae.EF4.74.dna.toplevel.shortChrNames.lengths

A file showing the lengths of the chromosomes in a table for the file `Saccharomyces_cerevisiae.EF4.74.dna.toplevel.shortChrNames.fa`.


*This READEME.md file was made with reference to the file of the same name in the 'input_annotation' folder of [Ssd1_CRACanalysis_2020 repository](https://github.com/ewallace/Ssd1_CRACanalysis_2020/tree/master/input_annotation)*