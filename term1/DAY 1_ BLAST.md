# Day 1: BLAST – Basic Local Alignment Search Tool

## Overview

This exercise introduces the Basic Local Alignment Search Tool (BLAST) and demonstrates how sequence similarity searches can be used to identify homologous sequences, interpret evolutionary relationships, and document findings using GitHub.

## Learning Objectives

- Understand what BLAST is and why it is important in bioinformatics.
- Perform a BLAST search using the NCBI BLAST interface.
- Interpret BLAST results using E-values, percentage identity, and bit scores.
- Differentiate between orthologs and paralogs.
- Document findings in a professional GitHub repository.

---

# Exercise 1: Getting Started with NCBI BLAST

## Objective

Navigate the NCBI BLAST interface and understand its components.

### Q1. What are the different BLAST programs available?

**Answer**

- BLASTN
- BLASTP
- BLASTX
- TBLASTN
- TBLASTX

### Q2. What is the default database used for nucleotide BLAST searches?

**Answer**

NCBI nucleotide database (`nr/nt`)

---

# Exercise 2: Human Insulin BLAST Search

## Objective

Search the human insulin coding sequence against the NCBI nucleotide database.

## Query Sequence

- **Gene:** INS (Human insulin)
- **Sequence type:** Coding DNA Sequence (CDS)
- **Length:** 333 bp

### BLAST Search Parameters

| Parameter | Value |
|-----------|-------|
| Program | BLASTN |
| Database | nr/nt |
| Query | Human INS CDS |

### Question

**What organism is the second match (after human)?**

**Answer**

*Gorilla gorilla gorilla*

---

# Exercise 3: Interpretation of BLAST Results

## Top BLAST Hits

| Hit | Organism | E-value | Identity (%) | Ortholog? |
|------|----------|---------|--------------|-----------|
| 1 | *Homo sapiens* (INS transcript variant 3) | 4e-171 | 100 | No |
| 2 | *Homo sapiens* (INS transcript variant 4) | 4e-171 | 100 | No |
| 3 | *Homo sapiens* (INS transcript variant 1) | 4e-171 | 100 | No |

### Q1. Are the top three hits orthologs or paralogs?

**Answer**

The top three hits represent transcript variants of the human INS gene. Since they originate from the same organism and correspond to alternative transcript variants of the same gene, they are not orthologs. They represent different transcript isoforms.

### Q2. What does the high percentage identity indicate?

**Answer**

The human insulin coding sequence is highly conserved.

### Q3. Why are these results biologically important?

**Answer**

Highly conserved genes can be used to study evolutionary relationships between species, identify homologous genes, and understand how essential biological functions have been maintained throughout evolution.

---

# Exercise 4: GitHub Documentation

## Repository Summary

The coding DNA sequence (CDS) of the human insulin (**INS**) gene was retrieved from NCBI Gene and analysed using **BLASTN** against the **NCBI nr/nt nucleotide database**. The top three BLAST matches corresponded to transcript variants of the human INS gene, each showing **100% sequence identity**, demonstrating strong conservation within the coding region. The closest non-human ortholog identified was *Gorilla gorilla gorilla*, exhibiting approximately **98.8% sequence identity**, highlighting the close evolutionary relationship between humans and gorillas.

---

# Reflection

## What was the most surprising discovery?

The presence of multiple human insulin transcript variants with identical coding sequences and the high similarity between human and gorilla insulin genes illustrate the remarkable evolutionary conservation of this essential gene.
