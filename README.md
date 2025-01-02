# Eye Conjunctivitis: Computational Modelling of Drug-Protein Interactions
## Overview
This project aims to identify potential therapeutic agents for adenovirus-induced conjunctivitis, focusing on computational methods to model drug-protein interactions. By integrating bioinformatics, cheminformatics, homology modeling, and molecular docking, the study seeks to develop targeted therapies for Ad64-induced viral conjunctivitis, commonly known as "pink eye."

# Key Features

## Drug-Protein Interaction Analysis:
* Examines interactions between eight drugs (e.g., Acyclovir, Ganciclovir, Erythromycin) and Ad64 proteins.
* Uses cheminformatics tools like RDKit and PyBioMed for molecular descriptor analysis.
  
## Protein Characterization:
* Analyzes Ad64 proteins, focusing on key targets such as the Hexon and Fiber proteins, using Amino Acid Composition (AAC) and Composition-Transition-Distribution (CTD) methods.

## Homology Modeling:
* Predicts 3D structures of Ad64 proteins using tools like MODELLER, Swiss-Model, and I-TASSER.
* Validates models with energy minimization and Ramachandran plots.
  
## Molecular Docking Simulations:
* Conducts docking studies using AutoDock Vina and PyRx to predict binding affinities and modes.
* Visualizes drug-protein interactions with PyMOL and Chimera.

## Ranking and Analysis:
* Ranks drugs based on binding affinities and interaction strengths, identifying the most promising candidates.

# Technologies and Tools
* Cheminformatics Tools: RDKit, PyBioMed
* Protein Modeling: MODELLER, Swiss-Model, I-TASSER
* Molecular Docking: AutoDock Vina, PyRx
* Visualization: PyMOL, Chimera
* Programming Languages: Python (NumPy, SciPy, Matplotlib)

# Project Objectives
* Develop a computational pipeline for drug discovery targeting Ad64.
* Predict drug-protein interactions using molecular docking.
* Identify potential therapeutic candidates for further experimental validation.
  
# Drugs and Their Properties

| Drug            | Interaction (%) | LabuteASA | TPSA   | Polarity   |
|-----------------|----------------|----------|-------|-----------|
| Erythromycin    | 89.86          | 303.595  | 193.91| High      |
| Tobramycin      | 79.71          | 185.051  | 268.17| High      |
| Ofloxacin       | 79.71          | 122.408  | 105.51| Moderate  |
| Ciprofloxacin   | 78.26          | 137.043  | 74.57 | Low       |
| Olopatadine     | 66.67          | 147.907  | 49.77 | Low       |

# Workflow

## Data Collection:
* Protein sequences from UniProt and NCBI.
* Drug structures from PubChem and DrugBank.

## Feature Extraction:
* Molecular descriptors (connectivity, topology, EState).
* Protein features (AAC, CTD).

## Modeling and Docking:
* Build 3D protein models.
* Simulate docking to evaluate drug binding.

## Analysis and Ranking:
* Rank drugs by binding affinity and interaction quality.

# Results
* Erythromycin demonstrated the highest binding affinity with Ad64 proteins.
* Visualization of drug-protein interactions revealed key residues involved in binding.
* Generated a comprehensive dataset of drug-protein interaction metrics.

 ![Alt Text]("C:\Users\chand\OneDrive\Pictures\Screenshots\Screenshot 2024-12-17 150856.png") 

# Future Directions
* Experimental validation of top drug candidates.
* Explore combination therapies for conjunctivitis.
* Expand methodologies to other viral infections.




## Final Results

| **Drug**         | **Interaction (%)** | **LabuteASA** | **TPSA**   | **Polarity**   | **Binding Affinity (kcal/mol)** |
|------------------|---------------------|---------------|------------|----------------|---------------------------------|
| **Erythromycin** | 89.86              | 303.595       | 193.91     | High           | -6.87                          |
| **Tobramycin**   | 79.71              | 185.051       | 268.17     | High           | -6.46                          |
| **Ofloxacin**    | 79.71              | 122.408       | 105.51     | Moderate       | -6.27                          |
| **Ciprofloxacin**| 78.26              | 137.043       | 74.57      | Low            | -6.26                          |
| **Olopatadine**  | 66.67              | 147.907       | 49.77      | Low            | -6.14                          |
| **Ganciclovir**  | 57.97              | 100.854       | 139.28     | Moderate       | -5.77                          |
| **Trimethoprim** | 50.73              | 122.408       | 105.51     | Moderate       | -6.15                          |
| **Acyclovir**    | 47.83              | 89.695        | 119.05     | Moderate       | -6.26                          |

---

### Highlights
- **Erythromycin** has the highest interaction percentage and strongest binding affinity.
- Drugs with higher polarity (LabuteASA/TPSA) may have better solubility but may require transporters for cell permeability.



# Conclusion
This project demonstrates how computational tools can help identify potential treatments for adenovirus-induced conjunctivitis. Using techniques like molecular docking, homology modeling, and descriptor analysis, we identified promising drug candidates such as Erythromycin and Tobramycin. These findings provide a strong foundation for further experimental validation and offer a cost-effective approach to drug discovery. This study can be extended to explore treatments for other viral infections in the future.
