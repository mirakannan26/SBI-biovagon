# SBI-biovagon

During the course of the internship, the core topics learnt were 
1. Databases (folder : Learning databases)
2. NGS Analysis
3. AI and ML for biology

## Databases

### BLAST – Insulin Sequence Homology Analysis

- Insulin CDS (coding sequence) of Homo sapiens was downloaded from NCBI.
- Nucleotide-nucleotide BLAST was performed (BLASTN) using NCBI’s BLAST, using 'nr/nt' as the database.
- Top 3 hits were found to be isoforms or alternative splice variants of the same gene in humans with a 100% query cover and percentage identity.
- Following the synthetic constructs, the first ortholog was that in Gorilla gorilla gorilla with a 98.8 % query cover.

**Biological meaning behind results** – the same INS gene produces multiple mRNA transcripts which are identical in their core coding exons but differ in their untranslated regions. Gorilla being the closest ortholog with a query cover of 100% and percentage identity of 98.8% shows a strong evolutionary relationship between Gorilla and Human.

### DNA Databases:

Exploration of the **human insulin (INS) gene** using genomic and variant databases. The exercises covered gene structure, genomic visualization, conservation and disease-associated variants.

**Tools & Databases**

- *Ensembl* – Gene structure, transcripts and genomic coordinates
- *UCSC Genome Browser* – Genomic context and conservation
- *ClinVar* – Disease-associated variants

**1. Ensembl**

Retrieved genomic information for the human INS gene:

- *Ensembl ID:* `ENSG00000254647`
- *Chromosome:* 11
- *Strand:* -
- *Coordinates:* 2,159,779–2,161,221
- *Transcript:* `ENST00000381330.5` (INS-202)

**2. UCSC Genome Browser**

Visualized INS using the *GRCh38/hg38* assembly and examined its genomic neighborhood.

- *Upstream:* `INS-IGF2`
- *Downstream:* `TH`
- Examined sequence conservation using the PhastCons track.

**3. ClinVar**

Investigated pathogenic insulin variants.

- *Variant:* `c.361G>A`
- *Disease:* Coronary artery disorder
- *Type:* Missense
- *Protein change:* `D121N`

**Key Learning Outcomes**

- Navigating Ensembl and UCSC Genome Browser
- Interpreting genomic coordinates, transcripts and exons
- Exploring genomic conservation
- Identifying disease-associated variants using ClinVar
- Connecting genomic organization with biological function

**Reflection**

The exercise demonstrated how BLAST and UCSC provide complementary perspectives: BLAST focuses on sequence similarity, while UCSC enables visualization of genomic context and comparative genomic features.

## RNA Database

The purpose of this exercise was to explore **RNAcentral** and understand its role in accessing, investigating, and visualising information related to RNA molecules and genes.

The exercise involved examining:

- RNA sequence and annotation information
- RNA and gene-related database records
- Links between information from different RNA resources
- RNA expression profiles
- Gene and RNA visualisation tools

## Learning Outcomes

The exploration of RNAcentral demonstrated the value of centralized databases for accessing information originating from multiple specialised resources.

The exercise provided an understanding of:

- RNA database organisation
- RNA sequence and annotation retrieval
- Gene and RNA expression information
- Biological data visualisation
- Integration of information from multiple databases

## Reflection

The exploration of RNAcentral demonstrated the importance of biological databases in organising and interpreting large volumes of biological information.

A key observation was that RNA databases can integrate different forms of information rather than functioning solely as sequence repositories. The availability of annotations, expression profiles, cross-references, and visualisation tools provides a more comprehensive view of RNA and gene-related data.

The examination of expression profiles also demonstrated how database resources can assist in identifying and interpreting patterns in biological data. Visualisation tools further support the interpretation of complex datasets by presenting biological information in an accessible format.

Overall, the exercise provided practical exposure to RNA databases, RNA information retrieval, gene expression profiles, database integration, and biological data visualisation.

### Protein Databases

Human insulin protein was analysed using UniProt, InterPro and the Protein Data Bank (PDB), focusing on protein annotation, conserved domains, structure and function.

**Tools & Databases**

- *UniProt* – Protein sequence, processing and annotations
- *InterPro / Pfam* – Conserved domains and protein families
- *PDB* – 3D protein structures

**1. UniProt**

Explored the reviewed human insulin entry:

- *Accession:* `P01308`
- *Entry:* `INS_HUMAN`
- *Length:* 110 aa
- *Signal peptide:* Residues 1–24
- *Processed chains:* A and B
- *Disulfide bonds:* 3

The processing of preproinsulin into mature insulin was also examined.

**2. Interpro**

Used InterPro to examine insulin's conserved family and compare it with IGF2. Both were associated with the insulin family and shared conserved features.

**3. PDB**

Explored a human insulin structure in PDB:

- *PDB ID:* `6RLX`
- *Method:* X-ray diffraction
- *Resolution:* 1.50 Å
- *Secondary structures:* α-helices and β-sheets
- *Oligomeric state examined:* Dimer

The relationship between insulin's zinc-stabilized hexameric storage form and its release as active monomers was also studied.

**Key Learning Outcomes**

- Interpreting UniProt protein records
- Understanding protein processing and conserved domains
- Exploring experimentally determined 3D structures
- Relating protein structure and oligomerization to function
- Connecting sequence variants with disease

**Reflection**

Studying protein structure provides insights beyond the amino-acid sequence by revealing domains, secondary structures, chains and oligomeric states that help explain biological function.

After the use of basic tools, a bioinformatic analysis on the resistance developed to the Gefitinib drug administered to patients having Non-small cell lung cancer, affected by a mutation in the gene synthesizing the Epidermal Growth Factor Receptor(EGFR) was performed as a project, utilizing the tools learned, with a few others.

## NGS Analysis

A complete RNA-Seq analysis workflow was carried out using **Galaxy**, starting from raw sequencing data and progressing through quality control, trimming, alignment, quantification, annotation and biological interpretation.

**Dataset**

- *Organism:* Drosophila melanogaster
- *GEO Accessions:* GSM461176, GSM461177, GSM461178, GSM461179
- *SRA Samples:* SRR031708, SRR031714, SRR031716, SRR031718
- *Parent Series:* GSE18508
- *Reference:* NCBI RefSeq, GCF_000001215.4
- *Annotation:* GTF

**Tools Used**

Galaxy | GEO | SRA | FastQC | Fastp | HISAT2 | Samtools | featureCounts | UniProt | FlyBase

**Next Generation Sequencing(NGS) pipeline :**

- Downloading datasets using SRA(NCBI)
- Checking quality of dataset using FASTQC tool with the quality metrics anaysis
- Trimming data using Trimmomatic tool in Galaxy (Fastp chosen later)
- FASTQC was used to check quality of trimmed data and compare with intial data
- Used HISAT2 to align the contigs generated from Trimmomatic (reference genome assembly)
- Samtools flagstat was used to check the quality of the aligned BAM files
- FeatureCounts was used for gene-level quantification of the aligned reads
- Top 10 expressed genes were identified based on their read counts
- UniProt and FlyBase were used to annotate the identified genes and understand their functions
- g:Profiler was attempted for functional annotation and GO analysis, but did not provide results
- FlyBase was used to obtain GO annotations for the top expressed genes
- Biological interpretation was performed based on the function and GO annotations of the top expressed genes

**Key Results**

FastQC showed a median quality of *Q30* across the samples. After trimming, read retention ranged from *97.56% to 99.84%*. HISAT2 alignment rates ranged from *65.89% to 90.84%*, with uniquely mapped reads ranging from *56.59% to 79.76%*.

FeatureCounts identified *9,737–10,325 genes with nonzero counts* across the four samples. The most highly expressed gene was *Dmel_CG8280 (eEF1alpha1)* in three samples, while *Dmel_CR34094 (mitochondrial large ribosomal RNA)* was highest in SRR031718.

**Biological Interpretation**

The top expressed gene in three samples, eEF1alpha1, is involved in *translation elongation and protein biosynthesis*. SRR031718 showed mitochondrial large ribosomal RNA as its top expressed feature, associated with *mitochondrial translation and ribosomal function*.

## Artificial Intelligence and Machine Learning in Biology

Different models trained to analyse biological data using machine learning

Difference between AI, ML and Deep Learning

Types of Machine learning - supervised, unsupervised and regression analysis
