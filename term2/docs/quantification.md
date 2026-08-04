# STAGE 8: QUANTIFICATION

## Tool Options

| Priority | Tool | Output |
|----------|------|--------|
| 1st option | featureCounts | Raw gene-level counts |
| 2nd option | HTSeq-count | Raw gene-level counts (equivalent output) |
| 3rd option | StringTie | TPM/FPKM and transcript-level abundance |

## Procedure

16. Provide the aligned BAM files and the GTF annotation from Stage 2 as input  
17. If the primary tool fails, proceed to the next option and record the reason for the change

**Attach:** quantification tool configuration and first rows of output table

After obtaining outputs for featurecount, counts data was downloaded:

[SRR031708_count](https://mirakannan26.github.io/SBI-biovagon/term2/reports/feature_counts_data/sheet001.html)         [SRR031714_count](https://mirakannan26.github.io/SBI-biovagon/term2/reports/feature_counts_data/SRR031714.csv)

[SRR031716_count](https://mirakannan26.github.io/SBI-biovagon/term2/reports/feature_counts_data/SRR031716.csv)         [SRR031718_count](https://mirakannan26.github.io/SBI-biovagon/term2/reports/feature_counts_data/SRR031718.csv)

| Field | Entry |
|-------|-------|
| Tool used | Feature Counts |
| Reason for tool selection | Being the 1st option, it performed the task and was hence chosen |
| Total genes with nonzero counts | Found using filter data option on galaxy:<br>SRR031708 – 9,737<br>SRR031714 – 10,280<br>SRR031716 – 10,290<br>SRR031718 – 10,325 |
