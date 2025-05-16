# Materials: Sequence Models


## Hands-on: Training a sequence-based model

Notebook: [01_training_sequence_model.ipynb](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/blob/main/05_sequence_models/02_ism_and_tfmodisco.ipynb)

### Data

The folder [01_data](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/blob/main/05_sequence_models/01_data/) contains the data used in this hands-on tutorial.

File name: ultra_k562_full.tsv.gz

Description: This file contains element headers, sequences, and 3 log2(RNA/DNA) values from a Massively Parallel Reporter Assay (MPRA) experiment [1] in K562 cells. 

The file is a tab-separated file with the following columns:

    - name: unique identifier for each element
    - sequence: DNA sequence of the element
    - log2.1: log2(RNA/DNA) value for the first replicate
    - log2.2: log2(RNA/DNA) value for the second replicate
    - log2.3: log2(RNA/DNA) value for the third replicate
    - log2.mean: mean of the three log2(RNA7DNA) values



## Hands-on: Interpreting models with in-silico mutagenesis

Notebook: [02_ism_and_tfmodisco.ipynb](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/blob/main/05_sequence_models/02_ism_and_tfmodisco.ipynb)

### Data

The folder [02_data](https://github.com/kircherlab/ISMB-2025_IGVF-MPRA-Tutorial/blob/main/05_sequence_models/02_data/) contains the data used in this hands-on tutorial.

1. [Agarwal, V., Inoue, F., Schubach, M. et al. Massively parallel characterization of transcriptional regulatory elements. Nature 639, 411–420 (2025).](https://doi.org/10.1038/s41586-024-08430-9)