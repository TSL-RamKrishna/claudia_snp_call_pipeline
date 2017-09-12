## Introduction

This is a rake pipeline to call SNPs. The pipeline does FASTQC on raw fastq data, trims out poor quality bases using trimmomatic, maps the high quality data to a reference sequence provided, generates mpileup with samtools mpileup and then calls SNPs using bcftools.

## Requirements

1. Ruby/Rake
2. FASTQC
3. Trimmomatic
4. Bowtie2
5. samtools
6. bcftools

## Usage:

rake -f rakefile R1=/path/to/R1.fastq R2=/path/to/R2.fastq reference=/path/to/refseq.fasta samplename=SampleA sampleid=Sample1

