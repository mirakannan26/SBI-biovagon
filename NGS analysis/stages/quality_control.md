# STAGE 3: QUALITY CONTROL

## Tool Options

| Priority | Tool |
|----------|------|
| Recommended | FastQC |
| Alternative (multi-sample summary) | MultiQC |

## Procedure

1. Run **FastQC** on each of the four raw FASTQ files.
2. Review the following quality metrics:
   - Per-base sequence quality
   - Adapter content
   - GC content
   - Sequence duplication level

## Attach

- FastQC summary report for each sample.

The FASTQ samples selected from the SRA corresponding to the GEO IDs **GSM461176**, **GSM461177**, **GSM461178**, and **GSM461179** were:

- **SRR031708**
- **SRR031714**
- **SRR031716**
- **SRR031718**

These FASTQ files were uploaded into **Galaxy**, and the **FastQC** tool was executed to generate quality control reports.

> **Note:** The selected SRR FASTQ files were chosen based on the metadata obtained from the **SRA Run Selector**.

## FastQC Reports

- [SRR031708](https://mirakannan26.github.io/SBI-biovagon/NGS%20analysis/reports/FASTQC_reports/SRR031708_fastq_fastqc.html)
- [SRR031714](https://mirakannan26.github.io/SBI-biovagon/NGS%20analysis/reports/FASTQC_reports/SRR031714_fastq_fastqc.html)
- [SRR031716](https://mirakannan26.github.io/SBI-biovagon/NGS%20analysis/reports/FASTQC_reports/SRR031716_fastq_fastqc.html)
- [SRR031718](https://mirakannan26.github.io/SBI-biovagon/NGS%20analysis/reports/FASTQC_reports/SRR031718_fastq_fastqc.html)

## Quality Control Summary

| Sample | Total Reads | Adapter % | Median Quality |
|--------|------------:|----------:|----------------|
| GSM461176 | 5,836,296 | 0% | Q30 (obtained from Per Base Sequence Quality) |
| GSM461177 | 10,654,850 | 0% | Q30 |
| GSM461178 | 11,843,414 | 0% | Q30 |
| GSM461179 | 6,724,171 | <5% | Q30 |
