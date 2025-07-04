# ISMB-2025_IGVF-MPRA-Tutorial

This is the main resource repository for the ISMB 2025 Tutorial IP2: Massively parallel reporter assays in functional regulatory genomics and as part of the IGVF data resource.

PDF conversions of the [preliminary slides are already available](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/tree/main/slides), but might change after the event based on corrections and feedback from participants.

We will work with Jupyter notebooks on Google Colab. If you would like to familiarize yourself with those, please check out: [https://colab.research.google.com/notebook
](https://colab.research.google.com/#scrollTo=GJBs_flRovLc)

If you want to make sure that you will be able to run these notebooks with your Google account, please try to start with the first [tutorioal](https://github.com/kircherlab/MPRAsnakeflow_tutorial/blob/main/tutorial_assignment.ipynb).

## Material

### [01 Introduction](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/tree/main/01_introduction)

### [02 Massively Parallel Reporter Assays (MPRAs)](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/tree/main/02_MPRAs)

### [03 Standard Pipeline for MPRA Analysis: MPRAsnakeflow](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/tree/main/03_MPRAsnakeflow)

#### External links:
- [MPRAsnakeflow repository](https://github.com/kircherlab/MPRAsnakeflow)
- [MPRAsnakeflow documentation](https://mprasnakeflow.readthedocs.io)
- [MPRAsnakeflow tutorial](https://github.com/kircherlab/MPRAsnakeflow_tutorial/)

#### Hands-on:
- **Association of Barcode/Tag Sequences**: [Jupyter/Colab notebook](https://github.com/kircherlab/MPRAsnakeflow_tutorial/blob/main/tutorial_assignment.ipynb)
- **Count Sequencing Analysis**: [Jupyter/Colab notebook](https://github.com/kircherlab/MPRAsnakeflow_tutorial/blob/main/tutorial_experiment.ipynb)

Output files are described in `03_MPRAsnakeflow/README.md`. Important results are copied to the `03_MPRAsnakeflow/assignment_workflow` and `03_MPRAsnakeflow/experiment_workflow` folders.

#### Discussion of QC metrics

We show the QC report of the 5' lentiMPRA from [Klein, J.C., Agarwal, V., Inoue, F. et al. A systematic evaluation of the design and context dependencies of massively parallel reporter assays. Nat Methods 17, 1083–1091 (2020).](https://doi.org/10.1038/s41592-020-0965-y). 

- [QC report assignment workflow](https://htmlpreview.github.io/?https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/blob/main/03_MPRAsnakeflow/qc_report.assignment.html)
- [QC report experiment workflow](https://htmlpreview.github.io/?https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/blob/main/03_MPRAsnakeflow/qc_report.experiment.html)

### [04 MPRA Data Analysis with BCalm](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/tree/main/04_MPRA_data_analysis)

#### Hands-on:
- **Data Analysis Steps (Regions and Variants)**: [README](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/blob/main/04_MPRA_data_analysis/README.md), [Jupyter/Colab notebook](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/blob/main/04_MPRA_data_analysis/04_mpra_analysis.ipynb)

### [05 Sequence Models](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/tree/main/05_sequence_models)

#### Hands-on:
- **Training a sequence-based model**: [Jupyter/Colab notebook](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/blob/main/05_sequence_models/01_training_sequence_model.ipynb)
- **Interpreting models with in-silico mutagenesis**: [Jupyter/Colab notebook](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/blob/main/05_sequence_models/02_ism_and_tfmodisco.ipynb)

### [06 Variant Effects and Motifs](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/tree/main/06_variant_effects_and_motifs)

#### Hands-on:
- **Linking motifs to variant effects**: [Jupyter/Colab notebook](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/blob/main/06_variant_effects_and_motifs/from_variant_effects_to_motifs.ipynb)
