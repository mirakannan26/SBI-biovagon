# STAGE 4: READ TRIMMING

## Tool Options

| Priority | Tool | Notes |
|----------|------|-------|
| 1st option | Trimmomatic | Standard adapter and quality trimming |
| 2nd option | Fastp | Faster, integrated QC and trimming |
| 3rd option | Cutadapt | Requires manual adapter sequence specification |

## Procedure

9. Attempt trimming with the recommended tool  
10. If the tool fails or produces errors, proceed to the next option in the table  
11. Apply a minimum quality threshold of **Q20** and a minimum read length of **36 bp**

**Attach:** trimming tool configuration and output summary

Tool : Fastp  
Version : 1.3.6

For datasets **SRR031708, SRR031718** – **45 cycles** [ mean length before filtering – 45 bp ]  
                                                [ mean length after filtering – 45, 43 bp respectively ]

**SRR031714, SRR031716** – **37 cycles** [ mean length before filtering – 37 bp ]  
                                             [ mean length after filtering – 36 bp ]

All datasets except the first (**SRR031708**) detected an adapter sequence.

| Field | Entry |
|-------|-------|
| Tool used | Fastp |
| Reason for tool selection | Trimmomatic displayed an error as it was unable to read the FASTQ file. Hence the next option, Fastp was used. |
| Sample | Reads Before | Reads After | % Retained |
| GSM461176 | 5.836296 M | 5.694161 M | 97.56 |
| GSM461177 | 10.654850 M | 10.584955 M | 99.34 |
| GSM461178 | 11.843414 M | 11.811890 M | 99.73 |
| GSM461179 | 6.724171 M | 6.713501 M | 99.84 |
