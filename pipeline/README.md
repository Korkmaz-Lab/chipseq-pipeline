## ChIP-seq Analysis Workflow

The ChIP-seq pipeline used in Korkmaz Lab follows a modular structure.
Not all steps are mandatory for every experiment.

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



