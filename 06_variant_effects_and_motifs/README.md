# Materials: Variant Effects and Motifs

Welcome! This directory contains resources and code for analyzing the effects of genetic variants on transcription factor binding motifs using MPRA data.
---

## Directory Overview

- **from_variant_effects_to_motifs.ipynb**
  *Main tutorial notebook:* Step-by-step workflow for linking variant effects to TF motifs, including data loading, FIMO analysis, and interpretation.
- **resources/**
  *Supporting data files:*
  - Motif databases (e.g., HOCOMOCO .meme files)
  - Example variant FASTA files
  - Metadata tables (variant and element info, gene activity matrices)
  - Images for illustration
---

## Outline

### 1. Introduction: Variants Tested with MPRA
- **Data sources:** MPRAsnakeflow results, Variant map, BCalm variant effects
- **Steps:**
    1. Normalize counts
    2. Run BCalm using normalized counts and variant map
    3. Identify significant variants

### 2. Transcription Factor Binding Motif Identification
- **Databases:**
  - JASPAR2022
  - HOCOMOCO v13
- **Tools:**
  - HOMER
  - FIMO (MEME suite)
- **Workflow:**
    - Run FIMO on test data
    - Merge TFBS information with variant metadata
    - Assess if TFBS are gained or lost due to variants
    - Increase confidence in TFBS calls (e.g., by filtering for cell-type expression)
    - Filter for variant-overlapping TFBS
    - Visualize the proportion of variants overlapping TFBS
---

## Getting Started

1. **Open the notebook:**
   `from_variant_effects_to_motifs.ipynb`
2. **Explore the resources:**
   Check the `resources/` folder for input data and motif files.
3. **Run the workflow:**
   Follow the notebook cells for a guided analysis.

For questions or suggestions, please contact the tutorial authors.