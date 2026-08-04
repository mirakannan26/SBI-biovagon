# STAGE 7: ALIGNMENT QUALITY CONTROL

## Tool Options

| Priority | Tool |
|----------|------|
| Recommended | Samtools flagstat |
| Additional | Samtools idxstats |
| Detailed QC | Qualimap BAMQC |
| RNA-specific QC | RSeQC |
| Visual inspection | IGV (desktop application) |

## Procedure

14. Run at least one BAM quality assessment tool on each aligned sample  
15. Optionally, load a BAM file in IGV to visually inspect read alignment at a gene of interest

**Attach:** BAM QC output (flagstat or equivalent)

For dataset **SRR031708**:  
BAM QC_SRR031708

For dataset **SRR031708**:  
BAM QC_SRR031714

For dataset **SRR031708**:  
BAM QC_SRR031716

For dataset **SRR031708**:  
BAM QC_SRR031718

| Field | Entry |
|-------|-------|
| Tool(s) used | Samtools flagstat |
| Observations | |

| Sample | Observation |
|--------|-------------|
| SRR031708 | Total reads: 7,652,014<br>Mapped reads: 5,709,817 (74.62%)<br>Primary mapped reads: 3,751,964 (65.89%)<br>Secondary alignments: 1,957,853 |
| SRR031714 | Total reads: 14900305<br>Mapped reads: 13930457 (93.49%)<br>Primary mapped reads: 9615107 (90.84%)<br>Secondary alignments: 4315350 |
| SRR031716 | Total reads: 15461466<br>Mapped reads: 13714190 (88.70%)<br>Primary mapped reads: 10064614 (85.21%)<br>Secondary alignments: 3649576 |
| SRR031718 | Total reads: 10208537<br>Mapped reads: 8534912 (83.61%)<br>Primary mapped reads: 5039876 (75.07%)<br>Secondary alignments: 3495036 |
