# piRNAnalyzer

piRNAnalyzer is a fully automated bash pipeline for the analysis of piRNAs in planarian small RNA Seq samples.

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

Required R packages will be downloaded automatically if not already installed on the user's system.

# How to use
1. Download the latest release of piRNAnalyzer and extract the zipped folder to the desired directory.
2. Copy raw data into the folder "01-Raw" within piRNAnalyzer's folder structure.
3. Invoke the bash script "piRNAnalyzer.sh". 

A sample dataset is available for download at [GSE192524](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE192524)

### Command Line Options
Flag | Function
-----|-----
`-h` | print this help message
`-p` | set the number of processor cores to be used (default: 4)
`-f` | setting filter options for preprocessing (default:all)	
Filter Options:| <table> <tbody> <tr> <td>`all`</td> <td>perform all filtering steps during preprocessing</td> </tr> <tr> <td>`rRNA`</td> <td>only perform rRNA filtering</td>  </tr> <tr> <td>`tRNA`</td> <td>only perform tRNA filtering</td> </tr> <td> `none` </td> <td>perform no additional filtering steps during preprocessing</td> </tr> </tbody> </table>
`-v` | print software version

# Citation
piRNAnalyzer is an automated version of the workflow presented in **DOI Will be added with link**.

Pittroff, A., Kim, I.V., Demtröder, T., Kuhn, C.D. (2022). Genome-wide analysis of planarian piRNAs. **EDIT CITATION DETAILS**  



