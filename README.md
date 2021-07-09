# piRNAnalyzer

piRNAnalyzer is a fully automated pipeline for the analysis of piRNAs in planarian small RNA Seq samples.

The piRNAnalyzer pipeline includes preprocessing of sequencing data, read mapping, annotation to genomic features, as well as quality control steps. It comes with all pre-built reference files necessary.


# Setup

Required third party programs
(please make sure that these are properly set up and can be invoked from the command line):

Software | Minimum version | Link
---------|-----------------|----------
Cutadapt | 1.15 | https://cutadapt.readthedocs.io/en/stable/
umitools | 0.2.0 | https://github.com/weng-lab/umitools
SortMeRNA | 2.1 | https://bioinfo.lifl.fr/RNA/sortmerna/
bowtie | 1.2.2 | http://bowtie-bio.sourceforge.net/index.shtml
piPipes | 1.5.0 | https://github.com/bowhan/piPipes
bedtools | 2.26.0 | https://bedtools.readthedocs.io/en/latest/
samtools | 1.7 | http://www.htslib.org/
bedGraphtoBigWig | - | https://genome.ucsc.edu/goldenpath/help/bigWig.html


# How to use
1. Download the piRNAnalyzer package and extract it to the desired directory
2. Copy your raw data into the folder "01-Raw"
3. Invoke the script "piRNAnalyzer.sh"

# Citation
Will be added


