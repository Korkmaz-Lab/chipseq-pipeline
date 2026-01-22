# Alignment

This step aligns ChIP-seq reads to the reference genome using Bowtie2.

---

## Purpose
- Map sequencing reads to the genome
- Generate an alignment file (SAM/BAM) for downstream processing

---

## Tool
- Bowtie2

---

## Inputs
- FASTQ files (raw or trimmed)
- Reference genome index (Bowtie2 index)

---

## Outputs
- SAM/BAM alignment files
- Alignment summary statistics (Bowtie2 log)

---

## Notes
- Use the correct genome build (e.g., hg38 or mm10) consistently across the project.
- Save Bowtie2 logs; they are useful for troubleshooting and reporting mapping rate.
