# SeqMule: Automated human exome/genome variants detection

SeqMule takes single-end or paird-end FASTQ or BAM files, generates a script consisting of more than 10 popular alignment, analysis tools and runs the script line by line. Users can change the pipeline or fine-tune the parameters by modifying its configuration file. SeqMule also has some built-in functions, such as pooling consensus calls from various callers, plotting a Venn diagram showing intersection among different callers, and downloading databases.

## Features

* Multiple aligners

   BWA-MEM, BWA-BACKTRACK, Bowtie, Bowtie2, SOAP2, SNAP

* Multiple variant callers

   GATK, SAMtools, VarScan, SOAPsnp, Freebayes are available.

   As stated on 1000 Genomes Project website, genotypes obtained through a consensus procedure are estimated to have 30% fewer errors than those generated by any single caller. 

   As we have demonstrated in a previous study (O'Rawe et al. *Genome Med* 2013, **5**:28), consensus calls from multiple calling algorithms may increase calling accuracy and reduce Mendelian error rates.

* Easy downloading and installation.

   Most jobs can be done with one-line command.

* Fast and easy customization

   Just change the 'advanced_config' file!


## Synopsis

* **seqmule download**: download databases/BEDs that are required by sequence alignment or variant calling software tools

* **seqmule pipeline**: perform the automated pipeline for detection of variants from whole-exome/genome data

* **seqmule stats**: perform statistical analysis of variants data, such as drawing Venn diagram to examine overlap between VCF files, generating union/consensus ca
lls, generating coverage/alignment statistics in specific genomic regions, calculating Mendelian error rates

* **seqmule run**: continue run from last executed step after interruption or run from a specific step

* **seqmule update**: perform automated update of the SeqMule software tools


## Revision History

For details, please go [here](https://github.com/WangGenomicsLab/SeqMule/commits/master)

## Contact

yunfeigu@usc.edu

Please join [SeqMule-dev](https://groups.google.com/forum/#!forum/seqmule-dev) for updates!

## More information

* [SeqMule Homepage](http://seqmule.usc.edu)

* [Wang Genomics Lab Homepage](http://genomics.usc.edu)



Copyright 2014 [USC Wang Lab](http://genomics.usc.edu)
