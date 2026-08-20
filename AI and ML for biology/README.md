# AI and Machine Learning for Biology

## Overview

This section documents the learning outcomes, key findings, and takeaways from a set of bioinformatics activities covering protein structure prediction, machine learning concepts, biomarker evaluation, and AI applications in biotechnology.

---

## Protein Structure Prediction with AlphaFold

### Learning Outcome
- Understand how AlphaFold predicts protein 3D structures from amino acid sequences.
- Interpret AlphaFold's pLDDT confidence scores and colour coding.
- Recognise the limitations of low-confidence or intrinsically disordered regions.
- Understand the relevance of predicted protein structures in drug discovery and biological research.

### Key Findings
- **Protein analysed:** EGFR receptor.
- The structure was predominantly **dark blue**, indicating high predicted confidence.
- Orange and yellow regions were observed in the peripheral and internal portions of the protein.
- Hemoglobin subunit beta showed higher overall confidence than EGFR, consistent with its small, compact, and well-defined structure and extensive experimental characterisation.

### Takeaway
AlphaFold provides rapid access to predicted protein structures, but confidence scores must be considered when interpreting specific structural regions, particularly for flexible or disordered portions.

---

## Machine Learning in Biological Data

### Learning Outcome
- Distinguish between **supervised and unsupervised learning**.
- Differentiate **classification, regression, and clustering** according to the type of biological problem being addressed.
- Understand how machine learning approaches can be applied to clinical, genomic, transcriptomic, and pharmaceutical datasets.

### Key Findings
The activity covered biological applications including:
- Tumour classification using labelled patient data.
- Clustering gene-expression profiles to identify hidden subtypes.
- Regression for predicting numerical traits such as age or hospital stay.
- Clustering of single-cell RNA-seq data to identify previously uncharacterised cell populations.
- Prediction of drug-trial outcomes from historical datasets.

### Takeaway
Selecting the appropriate machine learning approach depends on the structure of the data, the presence or absence of labels, and the type of output being predicted.

---

## Biomarker Evaluation

### Learning Outcome
- Evaluate a gene according to measurability, consistency, specificity, and potential actionability.
- Understand how gene-expression data can be considered in the context of biomarker discovery.
- Distinguish established clinical biomarkers from unsupported biomarker claims.

### Key Findings
- **Top expressed gene:** `Dmel_CG8280` from sample `SRR031708`.
- The encoded protein, Elongation factor 1-alpha 1, promotes the GTP-dependent binding of aminoacyl-tRNA to the A-site of ribosomes during protein biosynthesis.
- The gene was evaluated for measurable expression, consistency, specificity, and potential clinical actionability.
- Established examples identified included **PSA, HER2, HbA1c, and BRCA1/BRCA2**, while ZYX-9 Protein and NEUROFLEX-22 were classified as unsupported examples.

### Takeaway
High expression alone does not establish a gene as a useful biomarker. Clinical relevance depends on measurable, interpretable, and potentially actionable associations.

---

## AI Applications in Biotechnology

### Learning Outcome
- Explore how AI can be applied to multi-omics diagnostics and drug-response prediction.
- Identify the types of biological data required for AI-driven biotechnology.
- Consider challenges involving limited training data, prediction bias, ancestry-related variation, and experimental validation.
- Understand the role of virtual perturbation and structure-informed modelling in drug-response prediction.

### Key Findings
- **Proposed company:** Isotopic.
- **Focus:** Multi-Omics Diagnostics.
- Data sources considered included genomics, transcriptomics, proteomics, metabolomics, epigenomics, and protein structural information.
- Synthetic data generation using GANs and diffusion models was proposed for limited-data scenarios.
- Perturbation simulation was proposed to investigate the effects of mutations.
- The proposed workflow connects baseline omics data, an AI model, virtual perturbation, and predicted cellular outcomes.
- The concept also considers changes in receptor and drug conformation and the role of intramolecular strain energy.

### Takeaway
AI-driven biotechnology can integrate multiple biological data layers to model complex biological responses, but reliable applications require appropriate datasets, validation, and careful consideration of biological variation.
