# STAGE 4: READ TRIMMING

## Tool Options

| Priority | Tool | Notes |
|----------|------|-------|
| 1st option | Trimmomatic | Standard adapter and quality trimming |
| 2nd option | Fastp | Faster, integrated QC and trimming |
| 3rd option | Cutadapt | Requires manual adapter sequence specification |

## Procedure

1. Attempt trimming with the recommended tool.
2. If the tool fails or produces errors, proceed to the next option in the table.
3. Apply a minimum quality threshold of **Q20** and a minimum read length of **36 bp**.

## Attach

- Trimming tool configuration.
- Output summary.

### Tool Details

- **Tool Used:** Fastp
- **Version:** 1.3.6

### Reason for Tool Selection

Trimmomatic displayed an error as it was unable to read the FASTQ file. Therefore, the next recommended tool, **Fastp**, was used for read trimming.

### Trimming Summary

For datasets **SRR031708** and **SRR031718** (45 cycles):

- Mean read length before filtering: **45 bp**
- Mean read length after filtering:
  - **SRR031708:** 45 bp
  - **SRR031718:** 43 bp

For datasets **SRR031714** and **SRR031716** (37 cycles):

- Mean read length before filtering: **37 bp**
- Mean read length after filtering: **36 bp**

> **Note:** Adapter sequences were detected in all datasets except **SRR031708**.

## Read Trimming Statistics

| Sample | Reads Before | Reads After | % Retained |
|--------|-------------:|------------:|-----------:|
| GSM461176 | 5.836296 M | 5.694161 M | 97.56% |
| GSM461177 | 10.654850 M | 10.584955 M | 99.34% |
| GSM461178 | 11.843414 M | 11.811890 M | 99.73% |
| GSM461179 | 6.724171 M | 6.713501 M | 99.84% |
