# Single cell neuroblasts
Here I placed the notebooks I implemented to analize single-cell RNA sequencing data from insect neuroblasts
# Single-cell analysis of insect neuroblasts

This repository contains the computational workflows, analysis notebooks, and some of the processed results associated with the study of insect neuroblasts using single-cell RNA sequencing.

The analyses focus on the identification, annotation, comparison, and evolutionary analysis of neuroblast populations in *Drosophila melanogaster* and *Tribolium castaneum*. The repository includes workflows for transcription factor identification, species-specific single-cell analysis, integration of neuroblast datasets, cell-type annotation and label transfer, functional enrichment, differential expression analysis, and comparative analysis of transcription factor repertoires.

The repository is intended to provide the computational resources required to reproduce and inspect the analyses presented in the associated manuscript.

## Associated publication

**[MANUSCRIPT TITLE]**

[Author 1], [Author 2], [Author 3], **José Noel Sánchez Cabañas**, et al.

*Manuscript in preparation.*

The manuscript associated with this repository investigates the cellular and molecular evolution of insect neuroblasts using comparative single-cell transcriptomics.

> **Note:** The publication information will be updated with the final citation, DOI, and journal information upon publication.

## Repository organisation

The repository is organised according to the major stages of the analysis workflow.

### `1_TFs_predicted_and_annotated`

Identification and annotation of transcription factors used throughout the downstream analyses.

This directory contains:

* Predicted and annotated transcription factor sets for *Drosophila melanogaster*.
* Predicted and annotated transcription factor sets for *Tribolium castaneum*.
* Reference transcription factor lists compiled from multiple databases and published resources.
* A notebook documenting the pooling and selection of transcription factor candidates.

These resources provide the transcription factor sets used for subsequent comparative and differential-expression analyses.

### `2_Drosophila_NBs_initial_downstream_analysis`

Initial downstream analysis of the *Drosophila melanogaster* neuroblast single-cell dataset.

The notebooks include:

* Dataset cleaning and filtering.
* Initial dimensionality reduction and exploration of neuroblast populations.
* Manual annotation of *Drosophila* brain neuroblasts.

### `3_Tribolium_NBs_initial_downstream_analysis`

Initial downstream analysis of the *Tribolium castaneum* neuroblast single-cell dataset.

The notebooks include:

* Dataset cleaning and filtering.
* Initial dimensionality reduction and comparison of neuroblast populations.
* Manual annotation of *Tribolium* brain neuroblasts.

### `4_integration_Brain_NBs_datasets_and_annotation`

Integration and comparative annotation of brain neuroblast datasets from *Drosophila* and *Tribolium*.

This directory contains:

* The integration and label-transfer analysis notebook.
* Manual *Drosophila* brain neuroblast annotations.
* Resulting cell-type annotations obtained through cross-species label transfer.

This analysis provides the basis for comparing corresponding neuroblast populations between the two insect species.

### `5_gene_ontology_analysis`

Gene Ontology enrichment analyses associated with the identified neuroblast populations.

The directory contains:

* The Gene Ontology analysis notebook.
* Biological Process GO slim results.
* Molecular Function GO slim results.

### `6_pathways_enrichment_analysis`

Pathway-level functional analysis of genes associated with the analysed neuroblast populations.

The directory contains:

* A comprehensive gene-to-pathway annotation table.
* The notebook used for integrated pathway enrichment analysis of brain neuroblasts.

### `7_DE_analyses`

Differential expression analyses performed independently for *Tribolium* and *Drosophila* neuroblast datasets.

The directory is divided into:

* `1_Tribolium_DE_notebooks`
* `2_Drosophila_DE_notebooks`

The analyses include differential expression between brain neuroblasts and VNC neuroblasts, analyses based on different numbers of  pseudoreplicates, and analyses focused specifically on transcription factors, with separate analyses including or excluding Hox genes.

Processed differential-expression results are also provided as CSV files.

### `8_venn_diagrams_comparing_TFs_numbers`

Comparative analysis of transcription factor numbers identified across the different analyses and species.

This directory contains:

* Transcription factor sets identified in *Drosophila*.
* Transcription factor sets identified in *Tribolium*.
* TF sets including and excluding Hox genes.
* Results from analyses using different numbers of replicates.
* A notebook used to generate the Venn-diagram comparisons.

## Analysis workflow

The overall computational workflow can be summarised as:

1. **Transcription factor identification and annotation**
2. **Species-specific single-cell dataset preprocessing**
3. **Dimensionality reduction and neuroblast identification**
4. **Manual cell-type annotation**
5. **Cross-species dataset integration and label transfer**
6. **Gene Ontology enrichment**
7. **Pathway enrichment analysis**
8. **Differential expression analysis**
9. **Comparative analysis of transcription factor repertoires**

## Data availability

The notebooks in this repository contain the computational analyses and processed results associated with the study. The raw single-cell RNA-sequencing files  and the raw count matrices are available in the NCBI Geo database under: GSE337265.


## Reproducibility

The analyses are implemented primarily as Jupyter notebooks and use standard Python-based single-cell analysis workflows.

Because some analyses depend on external single-cell datasets, genome annotations, transcription factor databases, and pathway resources, users should consult the individual notebooks for the specific input datasets and resources used in each analysis.

## Repository status

This repository contains the analysis code and processed outputs associated with the manuscript.

The repository may be updated during manuscript preparation and following peer review to improve documentation, reproducibility, and alignment with the final published analyses.

## Citation

If you use the code or analyses provided in this repository, please cite the associated publication:

> [Full manuscript citation to be added upon publication.]

## License

This repository is distributed under the GNU General Public License v3.0 (GPL-3.0), as specified in the accompanying `LICENSE` file.

## Contact

For questions regarding the analyses or repository, please contact:

**Noel Cabañas**

Department of Zoology
University of Cambridge
United Kingdom
