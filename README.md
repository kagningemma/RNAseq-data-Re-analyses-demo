# RNAseq data re-analysis
The aim was to re-analyze published RNAseq differential expression dataset for comparison of gene expression between two kind of stem cells. 
The data was originally published in the paper https://www.nature.com/articles/s41467-019-10197-x

# Method
*Data retrieval* : I downloaded six fastq files related to this project from Gene expression Omnibus link provided earlier using SRA tools and CLC genomics v10 download tool. The hg38 version of the human genome, including various annotations were also downloaded from Ensembl website.

*Quality control* : Quality control of raw reads was done using fastQC, a snapshot of the results can be seen here. Based on that QC report, I trimmed the first 15 nt. I also filtered reads with PHRED score <20 and reads below 75 nucleotides of length.

*Reads mapping* : Mapping of the quality trimmed reads to the hg38 version of human genome was done.Reads’s alignement for each sample was done using CLC genomics v10 read mapper.  A file containing total read counts (generated by CLC genomics workbench V10) was imported into R for downstream statistical analyses.  

# How to view the data analysis report
- Step 1: Click on the "report.html" in the "RNAseq-data-Re-analyses-demo" directory of this repository
- Step 2: Right-click on the "Download" button and choose "save link as", then choose the directory where you would like to save it on your PC. 
- Step 3: Double-click on the html file to open it on your preferred browser

# Softwares
- R 
- CLC genomics 

# Computer
All analyses were performed on Ubuntu 18.04.5LTS operating system, memory 64GB, Intel Xeon(R) CPU v3 @ 1.6GHZ x 12, Graphics GeForce RTX 2080/PCIe/SSE2.


