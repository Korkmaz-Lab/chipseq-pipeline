# Downstream Analysis

This step covers downstream analyses performed after peak calling
to interpret ChIP-seq results in a biological context.

---

## Purpose
- Assign peaks to genomic features and genes
- Identify enriched DNA motifs
- Generate summary plots and visualizations

---

## Common Analyses
- Peak annotation (promoters, enhancers, intergenic regions)
- Motif enrichment analysis
- Signal aggregation and heatmaps
- Comparative visualization across conditions

---

## Tools
- HOMER
- R (e.g. ggplot2, ChIPseeker, deepTools)

---

## Inputs
- Peak files (MACS2 or THOR outputs)
- Reference genome annotations
- Signal tracks (bigWig)

---

## Outputs
- Annotated peak tables
- Motif enrichment results
- Publication-ready figures

---

## Notes
- Downstream analyses depend on the biological question.
- Tool choice and parameters may vary between projects.
- Results should always be interpreted together with QC metrics.
