# Overview

This repository contains the code and notebooks used to integrate the Kamath single-cell dataset into the MidMap atlas, a comprehensive reference of midbrain cell types. The project aims to address batch effects and technical discrepancies between datasets so that downstream analyses—such as differential gene expression studies in Parkinson’s disease—can be performed reliably. The integration process involves data concatenation, preprocessing, cell type annotation, and advanced integration techniques using tools such as scVI and Harmony.

# Repository Structure

- **/data** – Contains raw and processed data files.
- **/notebooks** – Jupyter notebooks detailing the workflow:
  - **0_creating_concatenated_anndataobj.ipynb**: Combines multiple anndata objects into one unified object.
  - **1_preprocessing_kamath.ipynb**: Performs quality control, filtering, and normalization of the Kamath dataset.
  - **4_label_metadata_integration.ipynb**: Integrates cell type labels and metadata with the MidMap atlas.
  - **5_integration_neuron_Kamath.ipynb**: Executes the initial integration of neuronal subsets from the Kamath dataset.
  - **6_integration_neuron_Kamath.ipynb**: Refines the neuronal integration and assesses batch effects.
- **/scripts** – Python scripts extracted from the notebooks (if available).
- **requirements.txt** – Lists all dependencies required to run the code.
- **README.md** – This file, which provides an overview and usage instructions.
