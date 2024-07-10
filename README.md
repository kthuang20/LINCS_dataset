This project uses the following resources:
- [LINCS L1000 dataset](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE70138)
- [Drug Repurposing Hub Indications](https://repo-hub.broadinstitute.org/repurposing#download-data)
- Indications of drugs in clinical trials from the AACT database


This GitHub repository contains the following jupyter notebooks:

* `1. Generating DRH datasets.ipynb` -- This notebook describes the steps taken to prepare the Drug Repurposing Hub (DRH) datasets later used to train the model.
* `2. Generating Connectivity Scores.ipynb` -- This notebook describes the steps taken to generate the file containing all the connectivity scores used to compare to our proposed model based on spearman correlation.
* `3. Preliminary Analysis (Fig 1).ipynb` -- This notebook compares the performance of a model based on connectivity scores vs. our proposed model and generates Figures 1a and 1b.
* `4. Exploring Impact of TAS (Fig 2).ipynb` -- This notebook describes the steps taken to compare how the TAS might affect the performance of our proposed model, generating Figures 2a and 2b.
* `5. Generating the Clinical Trials Datasets.ipynb` -- This notebook details the steps taken to generate the clinical trials datasets, later used to evaluate how well our model can predict for new uses of drugs.
* `6. Evaluate Model (Figure 3).ipynb` -- This notebook details the steps taken to generate the weighted average ensemble model combining predictions across all cell lines and evaluating its performance for new experimental uses. This notebook generates Figures 3a and 3b.


Other relevant information:
* The `conn_scores` folder contains the files used to generate the `conn_scores.txt` file used to generate Figure 1b.
* The `DRH_clin_data` folder contains the DRH datasets datasets used to train and evaluate the model
* The `ref_data` folder contains the files relevant to the LINCS L1000 dataset and files used to prepare the DRH and clinical trial datasets.
