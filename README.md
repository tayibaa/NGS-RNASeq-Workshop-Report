# NGS-RNASeq-Workshop-Report
This repository contains a detailed report on RNA-Seq data analysis using Next Generation Sequencing (NGS). It covers the complete workflow including quality control, read trimming, alignment, read counting, differential gene expression analysis, and pathway visualization using standard bioinformatics tools on the Galaxy platform.
# NGS WORKSHOP REPORT

## RNA-Seq Data Analysis Using Next Generation Sequencing (NGS)

---

## Aim
To understand and perform a basic RNA-Seq data analysis workflow using Next Generation Sequencing (NGS), including quality control, read trimming, alignment, read counting, and differential gene expression analysis.

---

## Introduction
Next Generation Sequencing (NGS) is a high-throughput sequencing technology that enables rapid sequencing of DNA and RNA. RNA sequencing (RNA-Seq) is a widely used NGS application for studying gene expression by sequencing cDNA derived from RNA samples.

This workshop focused on learning the complete RNA-Seq analysis pipeline and gaining hands-on experience with commonly used bioinformatics tools to analyze sequencing data and derive meaningful biological insights.

---

## Dataset Used
- Type: RNA-Seq data  
- Format: FASTQ files  
- Organism: Mouse (*Mus musculus*)  
- Source: Publicly available dataset  
- Samples: Control and treated samples  

---

## Tools and Software Used
- FASTQC – Quality assessment of raw sequencing data  
- Trim Galore – Trimming low-quality reads and adapter sequences  
- Bowtie2 – Alignment of reads to the reference genome  
- FeatureCounts – Counting reads mapped to genes  
- DESeq2 – Differential gene expression analysis  
- Galaxy Platform – Online bioinformatics analysis environment  

---

## Methodology / Workflow

### 1. Quality Control (FASTQC)
Raw FASTQ files were analyzed using FASTQC to assess sequencing quality. Parameters such as per-base sequence quality, GC content, sequence length distribution, and adapter contamination were examined.

---

### 2. Read Trimming (Trim Galore)
Trim Galore was used to remove adapter sequences and low-quality bases from the raw reads. This step improves data quality and ensures better alignment results.

---

### 3. Read Alignment (Bowtie2)
Cleaned reads were aligned to the reference mouse genome using Bowtie2. The output was generated in SAM/BAM format, and alignment statistics were checked to evaluate mapping efficiency.

---

### 4. Read Counting (FeatureCounts)
FeatureCounts was used to assign aligned reads to genomic features (genes). A gene count matrix was generated for downstream analysis.

---

### 5. Differential Gene Expression Analysis (DESeq2)
DESeq2 was used to normalize gene count data and compare control and treated samples. Differentially expressed genes were identified using log2 fold change and adjusted p-values.

---

### 6. Visualization and Functional Analysis
Heatmaps were generated to visualize gene expression patterns. KEGG pathway analysis was performed to identify biological pathways associated with the differentially expressed genes.

---

## Results
High-quality reads were obtained after trimming. Most reads aligned successfully to the reference genome. Several genes showed significant up-regulation and down-regulation. Heatmaps clearly differentiated control and treated samples, and KEGG analysis highlighted relevant biological pathways.

---

## Conclusion
This workshop provided practical experience in RNA-Seq data analysis using NGS. The step-by-step workflow demonstrated how raw sequencing data can be transformed into biologically meaningful information, which is essential in genomics and transcriptomics research.

---

## Learning Outcomes
- Understanding of NGS and RNA-Seq concepts  
- Practical experience with bioinformatics tools  
- Ability to perform RNA-Seq data analysis  
- Interpretation of differential gene expression results  

---

## References
- FASTQC Documentation  
- Trim Galore User Guide  
- Bowtie2 Manual  
- DESeq2 Bioconductor Package  
- Galaxy Platform Documentation  
