# SBI-biovagon

The course of the Summer Bioinformatics Internship, has helped gain knowledge on the following topics during these terms:

## Term 1 : Databases

### Learning Databases

A folder named **"Learning Databases"** was created to organize and document the work carried out while learning about different biological databases and their applications.

DNA databases - NCBI, UCSC Genome Browser, Ensembl, Clinvar

### BLAST – Insulin Sequence Homology Analysis

- Insulin CDS (coding sequence) of Homo sapiens was downloaded from NCBI.
- Nucleotide-nucleotide BLAST was performed (BLASTN) using NCBI’s BLAST, using 'nr/nt' as the database.
- Top 3 hits were found to be isoforms or alternative splice variants of the same gene in humans with a 100% query cover and percentage identity.
- Following the synthetic constructs, the first ortholog was that in Gorilla gorilla gorilla with a 98.8 % query cover.

**Biological meaning behind results** – the same INS gene produces multiple mRNA transcripts which are identical in their core coding exons but differ in their untranslated regions. Gorilla being the closest ortholog with a query cover of 100% and percentage identity of 98.8% shows a strong evolutionary relationship between Gorilla and Human.

### RNA Databases

RNA databases - primarily GEO

### Protein Databases

Protein Databases - Uniprot, PDB, Interpro

The term concluded with a project on DAY 5 which was a bioinformatic analysis on the resistance developed to the Gefitinib drug administered to patients having Non-small cell lung cancer, affected by a mutation in the gene synthesizing the Epidermal Growth Factor Receptor(EGFR).

## Term 2 : NGS

Various sequencing methods followed till date, and those preferred according to need

### Next Generation Sequencing(NGS) pipeline :

- Downloading datasets using SRA(NCBI)
- Checking quality of dataset using FASTQC tool with the quality metrics anaysis
- Trimming data using Trimmomatic tool in Galaxy (Fastp chosen later)
- FASTQC was used to check quality of trimmed data and compare with intial data
- Used HISAT2 to align the contigs generated from Trimmomatic (reference genome assembly)

## Term 3 : Artificial Intelligence and Machine Learning in Biology

Different models trained to analyse biological data using machine learning

Difference between AI, ML and Deep Learning

Types of Machine learning - supervised, unsupervised and regression analysis
