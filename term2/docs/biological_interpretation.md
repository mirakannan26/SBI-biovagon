# STAGE 10: BIOLOGICAL INTERPRETATION

This is the final stage. Everything so far quality control, trimming, alignment, quantification was preparation. Here, you turn your data into ONE clear biological statement about your sample.

## 10.1 The Question You Are Answering

"What is this sample doing the most, and what does that tell us biologically?"

You already have a count/abundance table from Stage 8, listing every gene and how many reads matched it. The gene with the highest count (TPM) is the one this sample is expressing the most.

## 10.2 Step 1 Find Your Top Expressed Gene

1. Open your Stage 8 output table (from featureCounts, HTSeq, or StringTie)
2. Sort the table by count (or TPM/FPKM, if using StringTie) highest to lowest
3. Ignore the very top rows if they are labelled things like "__no_feature", "__ambiguous", or "__too_low_aQual" these are technical categories, not real genes
4. The first real gene ID at the top of your sorted list is your Top Expressed Gene

**Attach: screenshot of your sorted table showing the top gene and its count/TPM**

For dataset SRR031708:

<div align="center">
  <img src="../images/top_expressed_genes/top%20expression%20for%20SRR031708.png" width="500">
</div>

For dataset SRR031714:

<div align="center">
  <img src="../images/top_expressed_genes/top%20expression%20for%20SRR031714.png" width="500">
</div>

For dataset SRR031716:

<div align="center">
  <img src="../images/top_expressed_genes/top%20expression%20for%20SRR031716.png" width="500">
</div>

For dataset SRR031718:

<div align="center">
  <img src="../images/top_expressed_genes/top%20expression%20for%20SRR031718.png" width="500">
</div>

| Field | Entry |
|-------|-------|
| Sample analyzed | SRR031708 |
| Top gene ID | Dmel_CG8280 |
| Count / TPM value | 49485 |

| Field | Entry |
|-------|-------|
| Sample analyzed | SRR031714 |
| Top gene ID | Dmel_CG8280 |
| Count / TPM value | 128128 |

| Field | Entry |
|-------|-------|
| Sample analyzed | SRR031716 |
| Top gene ID | Dmel_CG8280 |
| Count / TPM value | 146767 |

| Field | Entry |
|-------|-------|
| Sample analyzed | SRR031718 |
| Top gene ID | Dmel_CR34094 |
| Count / TPM value | 81082 |

## 10.3 Step 2 Find Out What This Gene Does

Use the same annotation tool from Stage 9.

5. In Galaxy, search "g: Profiler"
6. Input: your single top gene ID (just this one gene, not a list)
7. Select your organism (from Stage 1)
8. Execute, and review the returned gene name, description, and GO terms

**Attach: g:Profiler output for your top gene**

Since g profiler did not send output file from Galaxy, the g:profiler website was tried out but it too failed to give results. Hence Gene Ontology (GO) annotations were checked for in FlyBase.

Eg: for dataset SRR031708

<div align="center">
  <img src="../images/top_expressed_genes/GO%20annotation.png" width="500">
</div>

| Field | Entry |
|-------|-------|
| Gene name | eEF1alpha1 |
| Function/description | This protein(Elongation factor 1-alpha 1) promotes the GTP-dependent binding of aminoacyl-tRNA to the A-site of ribosomes during protein biosynthesis. |
| Relevant GO term(s) | Enables GTP binding, enables GTPase activity, enables translation elongation factor activity involved_in translational elongation, involved_in translation |

For samples SRR031708, SRR031714, SRR031716:

| Field | Entry |
|-------|-------|
| Gene name | eEF1alpha1 |
| Function/description | This protein(Elongation factor 1-alpha 1) promotes the GTP-dependent binding of aminoacyl-tRNA to the A-site of ribosomes during protein biosynthesis. |
| Relevant GO term(s) | Enables GTP binding, enables GTPase activity, enables translation elongation factor activity involved_in translational elongation, involved_in translation |

For samples SRR031718:

| Field | Entry |
|-------|-------|
| Gene name | mitochondrial large ribosomal RNA |
| Function/description | Its molecular function is described by: structural constituent of ribosome. It is involved in the biological process described with: mitochondrial translation; pole cell formation. |
| Relevant GO term(s) | enables structural constituent of ribosome, involved_in mitochondrial translation, involved_in pole cell formation |

## 10.4 Step 3 Write Your Conclusion

Fill in this single sentence using only what you found above:

> "This sample is mainly producing [gene name], which is known to [function] suggesting this sample/tissue is actively involved in [biological process]."

**Your completed conclusion sentence**

Samples SRR031708, SRR031714, SRR031716 are mainly producing eEF1alpha1, which is known to promotes the GTP-dependent binding of aminoacyl-tRNA to the A-site of ribosomes during protein biosynthesis, suggesting that these samples are actively involved in translational elongation and translation.

Sample SRR031718 is mainly producing mitochondrial large ribosomal RNA, which is known to enable structural constituent of ribosome, suggesting this sample is actively involved in mitochondrial translation and pole formation.
