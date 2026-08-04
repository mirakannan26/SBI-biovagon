# STAGE 9: ANNOTATION

## Tool Options

| Priority | Tool |
|----------|------|
| Recommended | g: Profiler |
| Alternative | Biomart |
| Manual lookup | UniProt |

## Procedure

18. Select the top 10 genes by expression from the Stage 8 output  
19. Submit the gene list to the annotation tool and retrieve gene names and functions

**Attach: annotation tool output table**

For step 18, Sort tool was used to view the gene IDs based on their read numbers which indicate expression levels:

| For dataset SRR031708 – | For dataset SRR031714 – |
|--------------------------|--------------------------|
| Dmel_CG8280<br>Dmel_CG11051<br>Dmel_CG2238<br>Dmel_CG17489<br>Dmel_CG10236<br>Dmel_CG7808<br>Dmel_CG14792<br>Dmel_CG4264<br>Dmel_CG7977<br>Dmel_CR34094 | Dmel_CG8280<br>Dmel_CG2238<br>Dmel_CG17489<br>Dmel_CG14792<br>Dmel_CG10236<br>Dmel_CG7808<br>Dmel_CG4264<br>Dmel_CG6378<br>Dmel_CG5502<br>Dmel_CG7977 |

| For dataset SRR031716 – | For dataset SRR031718 – |
|--------------------------|--------------------------|
| Dmel_CG8280<br>Dmel_CG17489<br>Dmel_CG2238<br>Dmel_CG14792<br>Dmel_CG7808<br>Dmel_CG4264<br>Dmel_CG6378<br>Dmel_CG5502<br>Dmel_CG10236<br>Dmel_CG7977 | Dmel_CR34094<br>Dmel_CG8280<br>Dmel_CG17489<br>Dmel_CG2238<br>Dmel_CG10236<br>Dmel_CG4027<br>Dmel_CG3523<br>Dmel_CG14792<br>Dmel_CG4264<br>Dmel_CG7808 |

After sorting, Select First tool was used to select the top 10 expressing genes.

Out of the selected genes from their expression levels, the unique IDs are as follows. Tool used was Uniprot (for the protein coding genes) and FlyBase (for non-coding genes). For Uniprot, swiss reviewed results were documented.

| Gene ID | Gene Name | Function |
|---------|-----------|----------|
| **1. Dmel_CG8280** | eEF1alpha1 | This protein(Elongation factor 1-alpha 1) promotes the GTP-dependent binding of aminoacyl-tRNA to the A-site of ribosomes during protein biosynthesis. |
| **2. Dmel_CG11051** | Nplp2 | Protein – neuropeptide-like 2<br><br>Molecular function – neuropeptide hormone activity<br>Biological function – humoral immune response, neuropeptide signalling pathway |
| **3. Dmel_CG2238** | eEF2 | Protein - Eukaryotic translation elongation factor 2<br>Catalyzes the GTP-dependent ribosomal translocation step during translation elongation. |
| **4. Dmel_CG17489** | RpL5 | Protein - Large ribosomal subunit protein uL18<br>Component of the ribosome, a large ribonucleoprotein complex responsible for the synthesis of proteins in the cell. |
| **5. Dmel_CG10236** | LanA | Protein - Laminin subunit alpha<br>Binding to cells via a high affinity receptor, laminin is thought to mediate the attachment, migration and organization of cells into tissues during embryonic development by interacting with other extracellular matrix components. |
| **6. Dmel_CG7808** | RpS8 | Protein - Small ribosomal subunit protein eS8<br>Component of the small ribosomal subunit. |
| **7. Dmel_CG14792** | sta | Protein - Small ribosomal subunit protein uS2<br>Required for the assembly and/or stability of the 40S ribosomal subunit. |
| **8. Dmel_CG4264** | Hsc70-4 | Protein - Heat shock 70 kDa protein cognate 4<br>ATP binding, hydrolysis. Heat shock protein binding, protein folding chaperone etc. |
| **9. Dmel_CG7977 (unreviewed)** | RpL23A | Protein - Ribosomal protein L23A, isoform A<br>Ribonucleoprotein, ribosomal protein, rRNA binding |
| **10. Dmel_CR34094** | mitochondrial large ribosomal RNA | Its molecular function is described by: structural constituent of ribosome. It is involved in the biological process described with: mitochondrial translation; pole cell formation. |
| **11. Dmel_CG6378 (unreviewed)** | SPARC | Protein - Secreted protein, acidic, cysteine-rich, isoform A<br>Calcium ion binding, anterior Malpighian tube development, basement membrane assembly, mesoderm development etc. |
| **12. Dmel_CG5502** | RpL4 | Protein - Large ribosomal subunit protein uL4<br>RNA binding, structural constituent of rubosome, cytoplasmic translation |
| **13. Dmel_CG4027** | Act5C | Protein - Actin-5C<br>Actins are highly conserved proteins that are involved in various types of cell motility and are ubiquitously expressed in all eukaryotic cells. |
| **14. Dmel_CG3523** | FASN1 | Protein - Fatty acid synthase<br>Fatty acid synthetase is a multifunctional enzyme that catalyzes the de novo biosynthesis of long-chain saturated fatty acids starting from acetyl-CoA and malonyl-CoA in the presence of NADPH. |
