# [![Build Status](https://travis-ci.org/Miachol/BioInstaller.svg)](https://travis-ci.org/Miachol/BioInstaller) [![License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](https://en.wikipedia.org/wiki/MIT_License) [![codecov](https://codecov.io/github/Miachol/BioInstaller/branch/master/graphs/badge.svg)](https://codecov.io/github/Miachol/BioInstaller) 

BioInstaller package
==============

## Introduction
Install and download massive bioinformatics analysis software and database, such as NGS analysis tools with its required database or/and refference, is still a task that need to spend a lot of time. 

Especialy, when start a NGS analysis work in a new computer or system, you need costs so much time and energy to 
 establish a complete set of softwares and dependce of a analysis pipeline and set the corresponding configuration file.

[BioInstaller](https://github.com/Miachol/BioInstaller) can be used to install these tools, dependences and databases in R conveniently.

## Repositories

### - Softwares

** Open Source **

Name | Version_Newest | Description
:---:|:---:|:---
[BWA](https://github.com/lh3/bwa) | 0.7.15 | Mapping low-divergent sequences against a large reference genome, such as the human genome
[STAR](https://github.com/alexdobin/STAR) | 2.5.2b | Ultrafast universal RNA-seq aligner
[bowtie](https://github.com/BenLangmead/bowtie) | 1.2.0 | An ultrafast memory-efficient short read aligner
[bowtie2](https://github.com/BenLangmead/bowtie2) | 2.3.0 | A fast and sensitive gapped read aligner
[tophat2](https://github.com/infphilo/tophat) | 2.1.1 | A fast splice junction mapper for RNA-Seq reads
[hisat2](https://github.com/infphilo/hisat2) | 2.0.5 | A fast splice junction mapper for RNA-Seq reads
[htslib](https://github.com/samtools/htslib) | 1.3.2 | C-library for handling high-throughput sequencing data
[samtools](https://github.com/samtools/samtools) | 1.3.1 | Mpileup and other tools for handling SAM, BAM, CRAM
[bcftools](https://github.com/samtools/bcftools) | 1.3.1 | Calling and other tools for handling VCF, BCF
[bedtools](https://github.com/arq5x/bedtools2) | v2.26.0 | A powerful toolset for genome arithmetic. [More](http://bedtools.readthedocs.io/en/latest/) detail.
[vcftools](https://github.com/vcftools/vcftools) | 0.1.14 | A set of tools written in Perl and C++ for working with VCF files, such as those generated by the 1000 Genomes Project
[picard](https://github.com/broadinstitute/picard) | 2.8.1 | A set of Java command line tools for manipulating high-throughput sequencing (HTS) data and formats
[pindel](https://github.com/genome/pindel) | 0.2.5b8 | Detect breakpoints of large deletions, medium sized insertions, inversions, tandem duplications and other structural variants at single-based resolution from next-gen sequence data
[lofreq](http://csb5.github.io/lofreq/) | 2.1.2 | Sensitive variant calling from sequencing data
[VarScan2](http://dkoboldt.github.io/varscan/) | 2.4.3 | Variant calling and somatic mutation/CNV detection for next-generation sequencing data
[freebayes](https://github.com/ekg/freebayes) | 1.1.0 | Bayesian haplotype-based polymorphism discovery and genotyping (Unsupported now)
[HTSeq](https://github.com/simon-anders/htseq) | 0.6.1p2 | A Python library to facilitate processing and analysis of data from high-throughput sequencing (HTS) experiments
[GMAP](http://research-pub.gene.com/gmap/) | 2017-02-15 | A Genomic Mapping and Alignment Program for mRNA and EST Sequences and Genomic Short-read Nucleotide Alignment Program
[MACS](https://github.com/taoliu/MACS) | 2015.4.20 | MACS -- Model-based Analysis of ChIP-Seq. [More](http://liulab.dfci.harvard.edu/MACS/) detail.
[Edean](http://www.genomic.ch/edena/) | V3.131028 | De novo short reads assembler
[ucsc_utils](http://hgdownload.cse.ucsc.edu/admin/exe/) | v344 | UCSC genome browser 'kent' bioinformatic utilities (blat, liftOver, and other command line utilities) are freely downloadable for academic, noncommercial, and personal use.
[FastQC](http://www.bioinformatics.bbsrc.ac.uk/projects/fastqc/) | 0.11.5 | A quality control tool for high throughput sequence data.

** Protected **

Name | Newest | Description |
---|---|---
[ANNOVAR](http://annovar.openbioinformatics.org/en/latest/) | 2017Feb15 | An efficient software tool to utilize update-to-date information to functionally annotate genetic variants detected from diverse genomes (including human genome hg18, hg19, hg38, as well as mouse, worm, fly, yeast and many others
[GATK](https://software.broadinstitute.org/gatk/) | 3.7 | Developed by the Data Science and Data Engineering group at the Broad Institute, the toolkit offers a wide variety of tools with a primary focus on variant discovery and genotyping. Its powerful processing engine and high-performance computing features make it capable of taking on projects of any size (Protected need install by change.info)
[MuTect](http://archive.broadinstitute.org/cancer/cga/mutect/) | 1.1.7 | A method developed at the Broad Institute for the reliable and accurate identification of somatic point mutations in next generation sequencing data of cancer genomes (Protected need install by change.info)


### - Dependences
Name | Version | Description
:--- |:--- | --- 
[gatk_bundle](ftp://gsapubftp-anonymous@ftp.broadinstitute.org/bundle/b36) | b36 | Includes the 1000 Genomes pilot b36 formatted reference sequence (human_b36_both.fasta) along with all lifted over VCF files. The refGene track and BAM files are not available. We only provide data files for this genome-build that can be lifted over "easily" from our master b37 repository. Sorry for whatever inconvenience that this might cause. Also includes a chain file to lift over to b37.
[gatk_bundle](ftp://gsapubftp-anonymous@ftp.broadinstitute.org/bundle/b37) | b37 |  The Standard Data Set pending completion of the Hg38 bundle
[gatk_bundle](ftp://gsapubftp-anonymous@ftp.broadinstitute.org/bundle/hg18) | hg18 | Includes the UCSC-style hg18 reference along with all lifted over VCF files. The refGene track and BAM files are not available. We only provide data files for this genome-build that can be lifted over "easily" from our master b37 repository. Sorry for whatever inconvenience that this might cause. Also includes a chain file to lift over to b37.
[gatk_bundle](ftp://gsapubftp-anonymous@ftp.broadinstitute.org/bundle/hg19) | hg19 | Includes the UCSC-style hg19 reference along with all lifted over VCF files.
[gatk_bundle](ftp://gsapubftp-anonymous@ftp.broadinstitute.org/bundle/hg38) | hg38 | This contains all the resource files needed for Best Practices short variant discovery in whole-genome sequencing data (WGS). Exome files and itemized resource list coming soon(ish).

### - Refference

Name | Version | Description
:--- |:--- | :--- 
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/hg19.tar.gz) | hg19 | H. sapiens, UCSC hg19 (HFM index for reference)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/hg38.tar.gz) | hg38 | H. sapiens, UCSC hg38 (HFM index for reference)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/hg38_tran.tar.gz) | hg38_tran | H. sapiens, UCSC hg38 and gene annotations referred to in [the Nature Protocol paper](http://ccb.jhu.edu/software/hisat2/index.shtml) (HGFM index for reference plus transcripts)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/grch37.tar.gz) | grch37 | H. sapiens, Ensembl GRCh37 (HFM index for reference)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/grch37_snp.tar.gz) | grch37_snp | H. sapiens, Ensembl GRCh37 (HGFM index for reference plus SNPs)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/grch37_snp_tran.tar.gz) | grch37_snp_tran | H. sapiens, Ensembl GRCh37 (HGFM index for reference plus SNPs and transcripts)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/grch37_tran.tar.gz) | grch37_tran | H. sapiens, Ensembl GRCh37 (HGFM index for reference plus transcripts)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/grch38.tar.gz) | grch38 | H. sapiens, Ensembl GRCh38 (HFM index for reference)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/grch38_snp.tar.gz) | grch38_snp | H. sapiens, Ensembl GRCh38 (HGFM index for reference plus SNPs)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/grch38_snp_tran.tar.gz) | grch38_snp_tran | H. sapiens, Ensembl GRCh38 (HGFM index for reference plus SNPs and transcripts)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/grch38_tran.tar.gz) | grch38_tran | H. sapiens, Ensembl GRCh38 (HGFM index for reference plus transcripts)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/mm10.tar.gz) | mm10 | M. musculus, UCSC mm10 (HFM index for reference)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/grcm38.tar.gz) | grcm38 | M. musculus, Ensembl GRCm38 (HFM index for reference)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/grcm38_snp.tar.gz) | grcm38_snp | M. musculus, Ensembl GRCm38 (HGFM index for reference plus SNPs)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/grcm38_snp_tran.tar.gz) | grcm38_snp_tran | M. musculus, Ensembl GRCm38 (HGFM index for reference plus SNPs and transcripts)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/grcm38_tran.tar.gz) | grcm38_tran | M. musculus, Ensembl GRCm38 (HGFM index for reference plus transcripts)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/bdgp6.tar.gz) | bdgp6 | D. melanogaster, Ensembl BDGP6 (HFM index for reference)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/bdgp6_tran.tar.gz) | bdgp6_tran | D. melanogaster, Ensembl BDGP6 (HGFM index for reference plus transcripts)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/ce10.tar.gz) | ce10 | C. elegans, UCSC ce10 (HFM index for reference)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/dm6.tar.gz) | dm6 | D. melanogaster, UCSC dm6 (HFM index for reference)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/r64.tar.gz) | r64 | S. cerevisiae, Ensembl R64-1-1 (HFM index for reference)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/r64_tran.tar.gz) | r64_tran | S. cerevisiae, Ensembl R64-1-1 (HGFM index for reference plus transcripts)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/rn6.tar.gz) | rn6 | R. norvegicus, UCSC rn6 (HFM index for reference)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/sc3.tar.gz) | sc3 | S. cerevisiae, UCSC sacCer3 (HFM index for reference)
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/wbcel235.tar.gz) | wbcel235 | C. elegans, Ensembl WBcel235
[hisat2_reffa](ftp://ftp.ccb.jhu.edu/pub/infphilo/hisat2/data/wbcel235_tran.tar.gz) | wbcel235_tran | C. elegans, Ensembl WBcel235 (HGFM index for reference plus transcripts)
[ucsc_reffa](http://hgdownload.cse.ucsc.edu/goldenPath/hg19/bigZips/chromFa.tar.gz) | hg19 | The assembly sequence in one file per chromosome. Repeats from RepeatMasker and Tandem Repeats Finder (with period of 12 or less) are shown in lower case; non-repeating sequence is shown in upper case.
[ucsc_reffa](http://hgdownload.cse.ucsc.edu/goldenPath/hg38/bigZips/hg38.chromFa.tar.gz) | hg38 | The assembly sequence in one file per chromosome. Repeats from RepeatMasker and Tandem Repeats Finder (with period of 12 or less) are shown in lower case; non-repeating sequence isshown in upper case.
[ensemble_GRCh37_reffa](ftp://ftp.ensembl.org/pub/release-75/fasta/homo_sapiens/dna/Homo_sapiens.GRCh37.75.dna.primary_assembly.fa.gz) | 75 | Primary assembly contains all toplevel sequence regions excluding haplotypes and patches. This file is best used for performing sequence similarity searches where patch and haplotype sequences would confuse analysis.
[ensemble_GRCh38_reffa](ftp://ftp.ensembl.org/pub/release-87/fasta/homo_sapiens/dna/Homo_sapiens.GRCh38.dna.primary_assembly.fa.gz) | 87 | Primary assembly contains all toplevel sequence regions excluding haplotypes and patches. This file is best used for performing sequence similarity searches where patch and haplotype sequences would confuse analysis.
