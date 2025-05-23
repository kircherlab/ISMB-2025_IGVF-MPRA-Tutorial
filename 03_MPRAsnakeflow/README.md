# Materials: MPRAsnakeflow

- [MPRAsnakeflow repository](https://github.com/kircherlab/MPRAsnakeflow)
- [MPRAsnakeflow documentation](https://mprasnakeflow.readthedocs.io)
- [MPRAsnakeflow tutorial](https://github.com/kircherlab/MPRAsnakeflow_tutorial/)

## Assignment Workflow

The folder `assignment_workflow` contains the main results of the MPRAsnakeflow assignment pipeline used in this tutorial:

- `assignment_workflow/qc_report.default.html`: Quality control report generated by the pipeline.
- `assignment_workflow/assignment_barcodes.default.tsv.gz`: Assignment of barcodes to oligos. The file has two columns: the barcode sequence and the oligo name from the design file.
    ```bash
    zcat assignment_workflow/assignment_barcodes.default.tsv.gz | head -n 5
    ```
    ```text
    AAAAAAAAAGAAGGG oligo_006589
    AAAAAAAAATCGATC oligo_006917
    AAAAAAAAATGATCT oligo_211468
    AAAAAAAACACATGA oligo_005412
    AAAAAAAACAGTAAG oligo_006290
    ```

## Experiment Workflow

The folder `experiment_workflow` contains the main results of the MPRAsnakeflow experiment pipeline used in this tutorial:

- `experiment_workflow/qc_report.HepG2.MPRAworkshop.default.html` and `experiment_workflow/qc_report.HepG2.MPRAworkshop.tutorialConfig.html`: Quality control reports generated by the pipeline. The `default` run requires a minimum of 10 barcodes per oligo. The `tutorialConfig` run allows a minimum of 5 barcodes per oligo.

- `experiment_workflow/reporter_experiment.barcode.HepG2.MPRAworkshop.default.all.tsv.gz`: This file contains the counts of barcodes observed in DNA/RNA for each replicate. This file is needed for analysis tools like BCalm that require barcode-level data. No filtering (`all`) was applied, so all barcodes per oligo are shown. The first column is the barcode sequence, the second is the oligo name, and the remaining columns are the counts of the barcodes in each replicate and modality.
    ```bash
    zcat experiment_workflow/reporter_experiment.barcode.HepG2.MPRAworkshop.default.all.tsv.gz | head -n 5
    ```
    ```text
    barcode	oligo_name	dna_count_1	rna_count_1	dna_count_2	rna_count_2	dna_count_3	rna_count_3
    ACCTAAGGAGATACG	oligo_002500	4	10	2	2		
    AGCACATCCGGTAAT	oligo_002500			1	1		
    TTATGATTGTAGATT	oligo_002500			1	4		
    CGTGAAAGTGATATG	oligo_002500			2	8	1	3
    ```

- `experiment_workflow/reporter_experiment.oligo.HepG2.MPRAworkshop.default.all.tsv.gz`, `experiment_workflow/reporter_experiment.oligo.HepG2.MPRAworkshop.default.min_oligo_threshold_10.tsv.gz`, and `experiment_workflow/reporter_experiment.oligo.HepG2.MPRAworkshop.tutorialConfig.min_oligo_threshold_5.tsv.gz`: These files aggregate counts per oligo. The `all` file contains all observed oligos, `default.min_oligo_threshold_10` contains only those with a minimum of 10 barcodes, and `tutorialConfig.min_oligo_threshold_5` contains only those with a minimum of 5 barcodes. The first column is the replicate (`1`, `2`, or `3`), the second is the oligo name, followed by DNA and RNA counts, then normalized DNA/RNA counts (counts per million), log2 fold change (activity), and the number of different barcodes observed for the oligo.
    ```bash
    zcat experiment_workflow/reporter_experiment.oligo.HepG2.MPRAworkshop.default.all.tsv.gz | head -n 5
    ```
    ```text
    replicate	oligo_name	dna_counts	rna_counts	dna_normalized	rna_normalized	log2FoldChange	n_bc
    1	oligo_002500	23	42	47.3914	30.8285	-0.6204	8
    1	oligo_002501:oligo_002502	10	25	27.4733	24.4671	-0.1672	6
    1	oligo_002503	14	24	32.9679	20.1329	-0.7115	7
    1	oligo_002504	1	2	16.484	11.7442	-0.4891	1
    ```

## QC Report Discussion

You can view the QC reports here:

- [QC report assignment workflow](https://kircherlab.github.io/mprasnakeflow/assignment.html)
- [QC report experiment workflow](https://kircherlab.github.io/mprasnakeflow/experiment.html)

For completness we also uploaded them in this repository (`qc_report.assignment.html` and `qc_report.experiment.html`)
