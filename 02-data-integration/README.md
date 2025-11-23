# Data Integration with MOFA

Dataset: HPO-GO (Gene Ontology)

Authors:    
Filippo Corti   
Carlotta Donato   
Giorgio Dal Santo   


## Repository structure:

- `/clusters` contains the raw csv data, with the clustering labels.
- `/model` contains the .hdf5 MOFA Model trained over the Dataset.
- The notebooks contains:
  - `training_with_mofa.ipynb`: dataset loading and training of a MOFA Model with 15 Latent Factors.
  - `mofa_analysis.ipynb`: downstream analysis of the MOFA Model, following the tutorial on the MOFA website.
  - `clustering.ipynb`: dataset loading and clustering (both of single Views and of the MOFA Matrix).
  - `cluster_analysis.ipynb`: analysis of the NMI across clusters. 
  - `consensus_analysis.ipynb`: analysis of the consensus across cluster assignments and drawing of the genes graph.
