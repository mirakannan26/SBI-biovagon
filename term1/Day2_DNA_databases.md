# DNA Databases: Genomic Context

## Hands-On Workbook

**Day 2 - Bioinformatics Internship 2026**

## Learning Objectives

1. Access and navigate Ensembl genome browser
2. Retrieve gene structure information (exons, introns, UTRs)
3. Use UCSC Genome Browser to visualize genomic context
4. Find and interpret variants in ClinVar
5. Connect genomic data to biological function

---

# Exercise 1: Navigating Ensembl

**Objective:** Retrieve insulin gene from Ensembl and document its genomic features.

## Part A: Access Ensembl and Search for Insulin Gene

1. Go to https://www.ensembl.org
2. Select 'Human' under 'Search for a species'
3. Search for 'insulin' in the search box
4. Click on 'INS' (Insulin gene) to open the gene page

**Q1:** What is the Ensembl gene ID for insulin?

**Answer:** ENSG00000254647(should start with ENSG)

---

## Part B: Retrieve Genomic Coordinates

On the insulin gene page, look for 'Location' section. Fill in the following:

| Field | Value |
|-------|-------|
| Chromosome | 11 |
| Start Position | 2,159,779 |
| End Position | 2,161,221 |
| Strand | - (+ or -) |

**Calculate:**

Gene length = End Position - Start Position = **1442 bp**

---

## Part C: Understanding Gene Structure

Click on 'Transcripts' or 'Exons' to view the gene structure. Complete the table:

| Exon # | Start | End | Length | Contains 5' UTR? |
|--------|-------|-----|--------|------------------|
| 1 ENSE00001938789 | 2,161,209 | 2,161,168 | 42 | Y |
| 2 ENSE00003494357 | 2,160,988 | 2,160,785 | 204 | Y |
| 3 ENSE00003901829 | 2,159,997 | 2,159,779 | 219 | Y |

Above table is for transcript

**ENST00000381330.5**
# Exercise 2: UCSC Genome Browser Visualization

**Objective:** Visualize insulin gene in genomic context and identify neighboring genes.

## Part A: Access UCSC and Locate Insulin Gene

1. Go to https://genome.ucsc.edu
2. Confirm genome is set to 'Human' and assembly is 'GRCh38/hg38'
3. In the search box, type your insulin coordinates from Ensembl: chr11:5246517-5249250
4. Click 'Go' or press Enter

**Q1:** What gene is located immediately upstream (left) of insulin? (Use the gene name or symbol)

**Answer:** INS-IGF2

---

**Q2:** What gene is located immediately downstream (right) of insulin?

**Answer:** TH gene

---

## Part B: Exploring Genomic Features

Look at the various tracks displayed in UCSC. You should see:

1. Genes (RefSeq genes, Ensembl genes)
2. Sequence conservation (PhastCons conservation track)
3. Repeats and structural variants

**Q3:** Is the insulin gene region highly conserved across species? (Look at conservation track - high dark bar = conserved)

**Answer:** Yes / No. Evidence: ________________yes________________________

# Exercise 3: Finding Variants in ClinVar

**Objective:** Search for disease-associated variants in the insulin gene.

1. Go to https://www.ncbi.nlm.nih.gov/clinvar
2. Search for: 'insulin' AND 'pathogenic'
3. Click on one of the pathogenic variants and read the details

**Q1:** Find ONE pathogenic insulin variant. What is the variant (e.g., c.123A>G) and what disease does it cause?

**Variant:** ________c.361G>A________________

**Disease:** Coronary artery disorder

---

**Q2:** Is this a missense, nonsense, or frameshift mutation? How can you tell?

**Answer:** Missense mutation according to the HGVS data given for molecular consequence and it is also mentioned that it is a single nucleotide variant which changes the protein to D121N.

Which is INS-202 out of the 4 protein coding transcripts of INS or insulin gene.

# Reflection

How does understanding the genomic structure of insulin help you understand BLAST results from Day 1?

Results of UCSC and BLAST when compared, give insights on the conservation of insulin gene. In BLAST, the results are shown based on similarity, and not based on species which is why multiple paralogs were seen before the first ortholog. But in UCSC, it doesn’t automatically display and needs to be enabled using the comparative genomics filter.
