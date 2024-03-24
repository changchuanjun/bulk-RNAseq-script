# bulk-RNAseq-script

The raw sequencing data were quality-controlled using fastp (version 0.22.0) with the default settings. Subsequently, the filtered reads were aligned to the reference genome using HISAT2 (version 2.2.1) with default parameters. The resulting SAM file, containing the aligned reads, was converted to BAM format, sorted, and indexed with SAMtools (version 1.18). Gene expression counts were extracted from the BAM files using featureCounts (version 1.6.2). Differential expression analysis was then performed using the R package DESeq2 (version 3.10).
