# Signal Track Generation

This step generates genome-wide signal tracks from processed BAM files
for visualization and quality assessment.

---

## Purpose
- Visualize ChIP enrichment across the genome
- Enable inspection in genome browsers (e.g. IGV, UCSC)
- Support quality control and comparative analyses

---

## Tools
- deepTools (bamCoverage)
- bedGraphToBigWig (UCSC tools)

---

## Inputs
- Filtered and deduplicated BAM files
- Reference genome chromosome sizes file

---

## Outputs
- Normalized signal tracks (bigWig format)
- Optional bedGraph files

---

## Notes
- Normalization methods (e.g. CPM, RPGC) should be chosen consistently.
- Signal tracks are used for visualization and are not used directly for peak calling.
