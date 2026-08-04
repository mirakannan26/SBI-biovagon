# STAGE 5: POST-TRIM VERIFICATION

Re-run the quality control tool used in Stage 3 on the trimmed FASTQ files to confirm improvement.

**Attach:** post-trimming FastQC report

For dataset **SRR031708**: [SRR031708](https://mirakannan26.github.io/SBI-biovagon/term2/reports/FASTQC_reports/SRR031708_fastqc_report_trimmed.html)  
For dataset **SRR031714**: [SRR031714](https://mirakannan26.github.io/SBI-biovagon/term2/reports/FASTQC_reports/SRR031714_fastqc_report_trimmed.html)   
For dataset **SRR031716**: [SRR031716](https://mirakannan26.github.io/SBI-biovagon/term2/reports/FASTQC_reports/SRR031716_fastqc_report_trimmed.html)    
For dataset **SRR031718**: [SRR031718](https://mirakannan26.github.io/SBI-biovagon/term2/reports/FASTQC_reports/SRR031718_fastqc_report_trimmed.html)  

| Metric | Dataset | Before Trimming | After Trimming |
|--------|---------|----------------:|---------------:|
| Adapter % | SRR031708 | Close to 0% | Close to 0% (no adapters to remove) |
| | SRR031714 | 0% | 0% |
| | SRR031716 | 0% | 0% |
| | SRR031718 | <5% | 0% |
| Median Quality | SRR031708 | Q30 | Q30 |
| | SRR031714 | Q30 | Q30 |
| | SRR031716 | Q30 | Q30 |
| | SRR031718 | Q30 | Q30 |
| Duplication % | SRR031708 | 2.82% | 1.63% |
| | SRR031714 | 45.04% | 44.91% |
| | SRR031716 | 44.88% | 44.86% |
| | SRR031718 | 21.3% | 21.62% |

Adapter % determined from Adapter Content Graph

Median Quality determined from Per Base Sequence Quality

Duplication % determined from Sequence Duplication Levels (100-percent of sequences deduplicated)
