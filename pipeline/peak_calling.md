# Peak Calling (Single-condition)

This step identifies enriched genomic regions (peaks) for each ChIP-seq
sample independently using MACS2.

---

## Purpose
- Detect regions of significant ChIP enrichment
- Generate peak sets for downstream and comparative analyses

---

## Tool
- MACS2

---

## Inputs
- Filtered and deduplicated BAM files
- Input/control BAM files
- Reference genome size

---

## Outputs
- Peak files (e.g. narrowPeak or broadPeak)
- Summits files
- MACS2 log files

---

## Notes
- MACS2 is used for single-condition peak detection.
- Appropriate input controls should be provided when available.
- Peak type (narrow vs broad) should match the target (e.g. TF vs histone marks).
