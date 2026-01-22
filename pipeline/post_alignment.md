# Post-alignment Processing

This step performs quality filtering and duplicate removal on aligned ChIP-seq reads.

---

## Purpose
- Remove low-quality alignments
- Eliminate PCR duplicates
- Improve signal-to-noise ratio before peak calling

---

## Tools
- samtools
- sambamba

---

## Inputs
- BAM files generated from alignment
- Mapping quality thresholds

---

## Processing Steps
1. Filter reads by mapping quality
2. Remove unmapped or secondary alignments
3. Mark or remove duplicate reads

---

## Outputs
- Filtered BAM files
- Deduplicated BAM files
- Alignment statistics after filtering

---

## Notes
- Mapping quality thresholds should be chosen based on experimental design.
- Duplicate removal is especially important for transcription factor ChIP-seq.
