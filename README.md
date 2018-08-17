# ChIP-seq_SE_methods_analysis
Here I investigated ChIP-seq methods in calling high quality super-enhancer regions, with variable acetylation, transcription factors, and peak calling methodologies. The genes associated with these regions (proximity) were mapped to expression data to observe functional significance - via fpkm, fold change, cell type specificity and intron/exon ratio.




## Workflow:
* ChIP-seq from SRA
* Trim, align, qc check
* Peak calling
* Combine .bed files for strict (at least 50% overlap) intersecting peaks with different transcription factor and acetylation combinations
* Combine .bam files to crate custom references
* Run ROSE (Rank Ordering of Super Enhancers) programme for SE (+TE) quantification
* Combine gene lists with fold-change and fpkm expression data (Th1 0-72hr) to observe expression of the SE genes
* Visualise trends and statistics between datasets


### Th1 T cell grouping:
  1. 1TF+H3K27ac (TBET)
  2. 3TF+H3K27AC (TBET, STAT1, STAT4)
  3. 3TF (TBET, STAT1, STAT4)
  4. Just H3K27ac
  * (+ all shared SEs across, and between these)
  
### Mammary epithelium grouping:
  1. 1TF (STAT5A)
  2. 1TF+H3K27ac (STAT5A)
  3. 2TF (STAT5A, GR)
  4. 2TF +H3K27AC (STAT5A, GR)
  5. Just H3K27ac
  * (+ all shared SEs across, and between these)
