# MidMap-Kamath-Integration
 Overview

 This repository contains the code and notebooks used to integrate the Kamath single-cell dataset into the MidMap atlas, a comprehensive midbrain cell type reference. The  project  focuses on addressing batch effects and technical discrepancies between datasets to enable robust downstream analyses, such as differential gene expression studies in   Parkinson’s Disease (PD).

 •	0_creating_concatenated_anndataobj.ipynb: Combines multiple anndata objects from different sources into one unified object.
	•	1_preprocessing_kamath.ipynb: Performs quality control, filtering, and normalization of the Kamath dataset.
	•	4_label_metadata_integration.ipynb: Integrates cell type labels and metadata from the Kamath dataset with the existing MidMap atlas.
	•	5_integration_neuron_Kamath.ipynb: Executes integration of neuronal subsets from the Kamath dataset using methods such as scVI and Harmony.
	•	6_integration_neuron_Kamath.ipynb: Further refines the integration by evaluating batch effects (e.g., zeroing out PC1 and PC2) to improve alignment.
