## ChIP-seq Analysis Workflow

![ChIP-seq pipeline overview](/docs/figures/chipseq_pipeline_overview.png)

**Figure 1.** Overview of the standardized ChIP-seq analysis workflow used in the Korkmaz Lab.
The pipeline follows a modular design, and not all steps are mandatory for every experiment.

### Software Versions

The software versions shown in the workflow diagram represent example
configurations used in the lab environment. Specific versions may vary
depending on the computational setup and are not strictly required.

### Tools used (core)

| Step | Purpose | Tool(s) |
|---|---|---|
| QC | Read quality assessment | FastQC, MultiQC |
| Optional preprocessing | Adapter/quality trimming (if needed) | Trim Galore, fastp |
| Alignment | Map reads to reference genome | Bowtie2 |
| Filtering & dedup | Remove low-quality/duplicates | samtools, sambamba |
| Signal tracks | Coverage tracks for visualization | bamCoverage (deepTools) / bedGraphToBigWig |
| Peak calling (single) | Peaks per sample/condition | MACS2 |
| Differential peaks | Differential binding/peaks between conditions | THOR |
| Downstream | Annotation, motifs, visualization | HOMER (+ R) |



### 1. Initial Quality Control
Raw sequencing reads are assessed to evaluate sequencing quality
and potential technical issues.

### 2. Read Preprocessing (Optional)
Adapter trimming and read filtering are applied only when required
based on quality control results.

### 3. Alignment
Reads are aligned to the reference genome using a short-read aligner.

### 4. Post-alignment Processing
Aligned reads are filtered by mapping quality and duplicate reads
are removed where appropriate.

### 5. Signal Track Generation
Normalized genome-wide signal tracks (e.g. bigWig) are generated
for visualization and quality assessment.

### 6. Peak Calling (Single Condition)
Enriched genomic regions are identified independently for each
ChIP sample using established peak-calling methods.

### 7. Differential Binding Analysis (Optional)
When comparative analysis between conditions is required,
differential peak calling is performed using THOR.

### 8. Downstream Analysis
Identified peaks are subjected to annotation, motif analysis,
and integrative downstream analyses.



