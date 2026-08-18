# EGFR SNP rs4947492 and Gefitinib Resistance in NSCLC

## Aim

To investigate whether the **EGFR SNP rs4947492** has a plausible direct or indirect role in **intrinsic resistance to the tyrosine kinase inhibitor (TKI) gefitinib** in non-small cell lung cancer (NSCLC), using a multi-database in-silico approach.

## Research Focus

The project focuses on understanding whether rs4947492 can influence gefitinib resistance through its **genomic location, regulatory effect on EGFR expression, or association with gene-expression changes in gefitinib-sensitive and resistant cells**.

The SNP was selected because previous literature reported an association with TKI treatment outcomes, while pooled analysis did not provide statistically significant evidence, leaving its biological role unresolved.

## Research Question

**Does EGFR SNP rs4947492 show plausible evidence of directly or indirectly contributing to intrinsic gefitinib resistance in NSCLC, or could its reported clinical association be explained by other factors?**

## Tools and Findings

### 1. dbSNP — Variant Identification and Annotation

**Usage:**  
dbSNP was used to determine the basic identity and genomic characteristics of rs4947492, including its chromosomal position, alleles, functional annotation, and minor allele frequency.

**Finding:**  
rs4947492 is located on **chromosome 7 at position 55,120,299 (GRCh38)**. The reference allele is **G**, with alternative alleles including A, C, and T. The database annotation indicated that the variant could be located within an intronic or 5′ UTR region. Its allele-frequency information also supported the possibility of population-level variation.

### 2. UCSC Genome Browser — Genomic Context

**Usage:**  
UCSC was used to visualize the exact position of rs4947492 within the **EGFR gene structure** and determine whether it occurs in an exon, intron, or splice-site region.

**Finding:**  
Across the EGFR transcript isoforms examined, rs4947492 was found to be an **intronic variant**, rather than a 5′ UTR variant. It was not located at an intron-exon boundary or obvious splice site. Therefore, it is unlikely to directly alter the EGFR amino acid sequence or protein structure.

### 3. GTEx — Regulatory/eQTL Analysis

**Usage:**  
GTEx was used to determine whether rs4947492 is associated with changes in **EGFR gene expression**, providing functional evidence for a potential regulatory role.

**Finding:**  
The SNP showed a significant association with EGFR expression, particularly in **adipose-subcutaneous tissue**. The negative NES values indicated that the allele associated with the negative effect direction was associated with relatively lower EGFR expression. The effect was modest, suggesting a potential regulatory rather than protein-altering effect.

### 4. GEO/GEO2R — Expression in Gefitinib-Sensitive and Resistant Cells

**Usage:**  
GEO was used to investigate whether **EGFR expression differs between gefitinib-sensitive and gefitinib-resistant NSCLC cell lines**, providing a further link between EGFR expression and drug resistance.

**Dataset:**  
**GSE156054**, containing parental and drug-resistant sublines including HCC827/HCC827-GR and PC9/PC9-GR.

**Finding:**  
GEO2R identified the top 250 differentially expressed genes. EGFR showed a difference in expression between the resistant and sensitive groups, with the expression pattern suggesting higher EGFR expression in the resistant group. However, the analysis was based on a **very small sample size**, resulting in statistically insignificant adjusted *p*-values. Therefore, the observed expression difference cannot be considered sufficient evidence for a relationship between rs4947492 and gefitinib resistance.

## Overall Result

The multi-database analysis suggests that **rs4947492 is unlikely to directly cause gefitinib resistance through a protein-altering mechanism**, because it is an intronic variant and does not alter the EGFR coding sequence or appear to directly disrupt a splice-site region.

However, GTEx provides evidence that the variant may have a **regulatory effect on EGFR expression**, indicating a possible indirect mechanism.

The GEO analysis showed an expression difference between gefitinib-sensitive and resistant cells, but the result was **statistically insignificant because of the small sample size**. Therefore, the available in-silico evidence does not establish that rs4947492 directly or indirectly causes gefitinib resistance.

## Final Conclusion

**Overall, rs4947492 has a plausible regulatory association with EGFR expression but insufficient evidence to establish it as a causal contributor to gefitinib resistance.** The findings therefore suggest that its previously reported association with TKI treatment outcome requires further experimental validation and larger clinical datasets before a definitive biological role can be assigned.

