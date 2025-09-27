#  RNA-Seq Differential Expression Analysis (Lung Cancer )

## Project Overview
This project demonstrates a complete **RNA-Seq analysis workflow** for identifying differentially expressed genes (DEGs) in lung cancer data.  
It covers raw data processing, alignment, quantification, and downstream analysis with visualization and functional enrichment.

---

##  Workflow
1. **Data Acquisition**  
   - Downloaded RNA-Seq data (SRA) from NCBI.  
   - Downloaded human reference genome (hg38).  

2. **Preprocessing & QC**  
   - Split SRA files using `sratoolkit`.  
   - Quality control with `FastQC`.  

3. **Alignment & Quantification**  
   - Indexed hg38 genome using **Subread**.  
   - Aligned reads with **Subjunc**.  
   - Generated count matrix using **FeatureCounts**.  

4. **Differential Expression Analysis (RStudio)**  
   - DESeq2 for DEG identification.  
   - Visualizations:  
     - **Volcano plots** for DEG distribution.  
     - **MA plot** for expression shifts.  
     - **GO enrichment** for biological processes.  
     - **KEGG pathway analysis** for pathway-level insights.  

---

##  Results
- Identified several **upregulated and downregulated genes**.  
- **GO enrichment** highlighted stress response, protein folding, and cell fusion processes.  
- **KEGG analysis** pointed to canonical lung cancer pathways (cell cycle, PI3K-Akt, p53).  
- **Visualizations** (Volcano, MA, GO, KEGG) illustrate the transcriptional shifts.  

---

## Tools & Dependencies
- **sratoolkit** (for SRA download and splitting)  
- **FastQC** (quality control)  
- **Subread / Subjunc** (alignment)  
- **FeatureCounts** (read quantification)  
- **RStudio** with packages:  
  - `DESeq2`  
  - `ggplot2`  
  - `clusterProfiler`  
  - `org.Hs.eg.db`  

---

## 📂 Repository Structure
