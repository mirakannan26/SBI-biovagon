# BLAST: Basic Local Alignment Search Tool

## Hands-On Workbook

### Day 1 - Bioinformatics Internship 2026

## Learning Objectives

- Understand what BLAST is and why it matters in bioinformatics
- Perform a BLAST search using NCBI BLAST interface
- Interpret BLAST results: E-values, identity %, bit scores
- Identify and analyze orthologs and paralogs
- Document findings in a professional GitHub repository

---

# Exercise 1: Getting Started with NCBI BLAST

**Objective:** Navigate NCBI BLAST and understand the interface.

## Part A: Access NCBI BLAST

Go to https://blast.ncbi.nlm.nih.gov/Blast.cgi and answer the following questions:

### Q1: What are the different BLAST programs available? List at least 4.

**Answer:**

blastn,blastp,blastx,tblastn,tblastx

### Q2: Name the default database used for nucleotide BLAST searches.

**Answer:**

NCBI

---

## Part B: E-value Interpretation Challenge

Match each E-value to its interpretation:

| E-value | Your Answer | Correct Answer |
|---------|-------------|----------------|
| 3e-45 | True homolog | High similarity |
| 0.45 | Low significance | Low significance |
| 0.003 | High similarity | True homolog |

---

# Exercise 2: Run Your First BLAST Search

**Objective:** Search the human insulin gene sequence against NCBI databases.

## Step 1: Get the Insulin Gene Sequence

1. Go to NCBI Gene (https://www.ncbi.nlm.nih.gov/gene/)
2. Search for: 'insulin human' or 'INS gene'
3. Click on the first result (human insulin)
4. Under 'FASTA sequences', click 'CDS FASTA' to get the protein-coding sequence

### Q1: What is the length (in base pairs) of the human insulin CDS?

**Answer:** 333bp

### Human insulin CDS -

```fasta
>lcl|AH002844.2_cds_AAA59172.1_1 [gene=INS] [db_xref=GDB:G00-119-349] [protein=insulin] [protein_id=AAA59172.1] [location=join(2424..2610,3397..3542)] [gbkey=CDS]

ATGGCCCTGTGGATGCGCCTCCTGCCCCTGCTGGCGCTGCTGGCCCTCTGGGGACCTGACCCAGCCGCAG
CCTTTGTGAACCAACACCTGTGCGGCTCACACCTGGTGGAAGCTCTCTACCTAGTGTGCGGGGAACGAGG
CTTCTTCTACACACCCAAGACCCGCCGGGAGGCAGAGGACCTGCAGGTGGGGCAGGTGGAGCTGGGCGGG
GGCCCTGGTGCAGGCAGCCTGCAGCCCTTGGCCCTGGAGGGGTCCCTGCAGAAGCGTGGCATTGTGGAAC
AATGCTGTACCAGCATCTGCTCCCTCTACCAGCTGGAGAACTACTGCAACTAG
```

---

## Step 2: Set Up BLAST Search

5. Copy the CDS sequence (FASTA format with sequence ID)
6. Go to NCBI BLAST (https://blast.ncbi.nlm.nih.gov)
7. Click 'BLASTN' (nucleotide-nucleotide BLAST)
8. Paste your sequence in the 'Enter query sequence' box
9. Keep database as 'nr/nt'

### Q2: What organism is the second match (after human)?

**Answer:** Gorilla gorilla gorilla

---

## Step 3: Interpret Your Results

Complete the following table for the top 3 BLAST hits:

| Hit # | Organism | E-value | Identity % | Ortholog? |
|-------|----------|----------|------------|-----------|
| 1 | Homo sapiens insulin (INS), transcript variant 3, mRNA | 4e-171 | 100 | none |
| 2 | Homo sapiens insulin (INS), transcript variant 4, mRNA | 4e-171 | 100 | none |
| 3 | Homo sapiens insulin (INS), transcript variant 1, mRNA | 4e-171 | 100 | none |

---

# Exercise 3: Analysis and Interpretation

### Q1: Are the top 3 hits orthologs or paralogs of human insulin? Explain why.

**Answer:**

Paralogs as the 3 hits are variants of the same gene in the same organism and have different locus ids(on checking the individual accession ids). This indicates they have been duplicated during evolution.

### Q2: What does the high identity % in the top hit tell us about conservation of the insulin sequence?

**Answer:**

It is highly conserved

### Q3: Why would an evolutionary biologist be interested in these BLAST results?

**Answer:**

To compare similarity between species based on conservation of the gene and %identity and use that similarity to identify presence of metabolites and other gene products which may have been produced by older species. It can also be used to study phylogenetic relationships and compare ancient and more evolved organisms.

---

# Exercise 4: GitHub Documentation

**Objective:** Document your BLAST findings professionally.

Write a brief README section (200-300 words) for your GitHub repository describing:

- What sequence you searched
- What BLAST program and database you used
- Summary of top 3 hits
- Key biological insights from the results

## Your GitHub README Draft:

Insulin CDS (coding sequence) of Homo sapiens was downloaded from NCBI.

Nucleotide-nucleotide BLAST was performed (BLASTN) using NCBI’s BLAST, using 'nr/nt' as the database.

Top 3 hits were found to be isoforms or alternative splice variants of the same gene in humans with a 100% query cover and percentage identity.

Following the synthetic constructs, the first ortholog was that in Gorilla gorilla gorilla with a 98.8 % query cover.

Biological meaning behind results – the same INS gene produces multiple mRNA transcripts which are identical in their core coding exons but differ in their untranslated regions. Gorilla being the closest ortholog with a query cover of 100% and percentage identity of 98.8% shows a strong evolutionary relationship between Gorilla and Human.

---

# Reflection Questions

### What was the most surprising discovery from your BLAST results?

That insulin had these many variants and they all showed a 100% similarity. Also the fact that Gorilla showed 98.8% similarity to human insulin, in a way indicating their evolutionary relationship.
