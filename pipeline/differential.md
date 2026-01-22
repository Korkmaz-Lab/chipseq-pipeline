# Differential Binding Analysis

This step identifies differential ChIP enrichment between experimental
conditions using a comparative peak calling approach.

---

## Purpose
- Detect condition-specific or differential binding events
- Compare ChIP signal across biological replicates and conditions

---

## Tool
- THOR

---

## When to Apply
- When at least two experimental conditions are available
- When biological replicates are present
- When input/control samples are available

---

## Inputs
- Processed BAM files from multiple conditions
- Input/control BAM files
- Experimental design information

---

## Outputs
- Differential peak sets
- Condition-specific peaks
- Statistical significance scores

---

## Notes
- THOR is used only for differential binding analysis.
- It is not a replacement for single-condition peak calling.
- Proper experimental design is critical for reliable results.
