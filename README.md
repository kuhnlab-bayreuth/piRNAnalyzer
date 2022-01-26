# piRNAnalyzer

piRNAnalyzer is a fully automated pipeline for the analysis of piRNAs in planarian small RNA Seq samples.

The piRNAnalyzer pipeline includes preprocessing of sequencing data, read mapping, annotation to genomic features, as well as quality control steps. It comes with all pre-built reference files necessary.


# Setup

Required third party programs
(please make sure that these are properly set up and can be invoked from the command line):

Software | Minimum version | Link | Command Line Invocation
---------|-----------------|----------|--------------------
Cutadapt | 1.15 | https://cutadapt.readthedocs.io/en/stable/ | cutadapt
umitools | 0.2.0 | https://github.com/weng-lab/umitools | umitools reformat_sra_fastq
SortMeRNA | 2.1 | https://bioinfo.lifl.fr/RNA/sortmerna/ | sortmerna
bowtie | 1.2.2 | http://bowtie-bio.sourceforge.net/index.shtml | bowtie
piPipes | 1.5.0 | https://github.com/bowhan/piPipes | piPipes_fastq_to_insert, piPipes_insertBed_to_bed2
bedtools | 2.26.0 | https://bedtools.readthedocs.io/en/latest/ | bedtools
samtools | 1.7 | http://www.htslib.org/ | samtools
bedGraphtoBigWig | - | https://genome.ucsc.edu/goldenpath/help/bigWig.html | bedGraphToBigWig
R | 4.1.2 | https://www.r-project.org/ | R 


# How to use
1. Download the latest release of piRNAnalyzer and extract the zipped folder to the desired directory.
2. Copy raw data into the folder "01-Raw" within piRNAnalyzer's folder structure.
3. Invoke the bash script "piRNAnalyzer.sh".

# Citation
Will be added


