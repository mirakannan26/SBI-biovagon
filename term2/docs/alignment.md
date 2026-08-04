# STAGE 6: ALIGNMENT

## Tool Options

| Priority | Tool | Notes |
|----------|------|-------|
| Recommended (RNA-Seq) | HISAT2 | Splice-aware aligner |
| Alternative | STAR | Splice-aware, higher memory requirement |
| Not recommended for RNA-Seq | BWA-MEM | DNA aligner, not splice-aware |

## Procedure

12. Align each trimmed FASTQ file to the reference genome obtained in Stage 2  
13. Record the alignment summary statistics for each sample

**Attach:** alignment summary output for each sample

For dataset SRR031708:  
[SRR031708_alignment_summary](https://mirakannan26.github.io/SBI-biovagon/term2/reports/alignment_summary/SRR031708_alignment_summary.txt)

For dataset SRR031714:  
[SRR031714_alignment_summary](https://mirakannan26.github.io/SBI-biovagon/term2/reports/alignment_summary/SRR031714_alignment_summary.txt)

For dataset SRR031716:  
[SRR031716_alignment_summary](https://mirakannan26.github.io/SBI-biovagon/term2/reports/alignment_summary/SRR031716_alignment_summary.txt)

For dataset SRR031718:  
[SRR031718_alignment_summary](https://mirakannan26.github.io/SBI-biovagon/term2/reports/alignment_summary/SRR031718_alignment_summary.txt)

| Sample | Tool Used | Overall Alignment % | Uniquely Mapped % |
|--------|-----------|--------------------:|------------------:|
| GSM461176<br>(SRR031708) | HISAT2 | 65.89% | 56.59% |
| GSM461177<br>(SRR031714) | HISAT2 | 90.84% | 79.76% |
| GSM461178<br>(SRR031716) | HISAT2 | 85.21% | 76.66% |
| GSM461179<br>(SRR031718) | HISAT2 | 75.07% | 61.15% |
