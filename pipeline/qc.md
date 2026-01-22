# Quality Control & Read Preprocessing

This step evaluates raw ChIP-seq reads for sequencing quality and
identifies potential technical issues prior to alignment.

---

## Quality Control (mandatory)

**Purpose**
- Assess base quality, GC content, adapter contamination
- Detect overrepresented sequences and technical artifacts

**Tools**
- FastQC
- MultiQC

**Outputs**
- Individual FastQC reports (`*.html`)
- Aggregated MultiQC report (`multiqc_report.html`)

---

## Read Preprocessing (optional)

Read trimming is applied **only if required**, based on QC results.

**When to apply**
- Adapter contamination detected
- Low-quality bases at read ends
- Abnormal per-base quality profiles

**Tools**
- Trim Galore
- fastp

**Outputs**
- Trimmed FASTQ files
- Updated QC reports (recommended)

---

## Notes
- Trimming is not mandatory for all datasets
- Over-trimming should be avoided to preserve signal
