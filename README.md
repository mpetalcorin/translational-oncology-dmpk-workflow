# translational-oncology-dmpk-workflow
A proof-of-concept oncology DMPK workflow that integrates simulated ADME and translational PK data, machine learning, candidate ranking, and simplified PK/PD modelling for developability assessment.

<img width="702" height="986" alt="Screenshot 2026-04-10 at 02 37 02" src="https://github.com/user-attachments/assets/6938f523-163f-4de3-89e2-43cca205786e" />

# Simulated Translational Oncology DMPK Workflow
## Overview
This repository contains a proof-of-concept translational oncology DMPK project built around a simulated portfolio of compounds. The workflow integrates literature-benchmarked ADME and pharmacology variables, exploratory analysis, machine learning, candidate ranking, and simplified PK/PD scenario modelling to demonstrate how DMPK evidence can support candidate selection and human translation.

## Repository contents
- `principal_scientist_dmpk_oncology_proof_of_concept.ipynb`
- `README.md`, project overview and usage guide.
- `modelcard.md`, intended use, assumptions, metrics, and limitations of the predictive models.
- `datasheet.md`, documentation for the simulated dataset and derived variables.

## Scientific goal
The goal is to show how a translational DMPK workflow can move from early assay-style measurements to interpretation, machine learning-assisted triage, human PK projection, and mechanistically guided candidate prioritisation in oncology.

## Workflow summary
Steps:
1. Simulates an oncology compound portfolio using literature-style ranges for physicochemical, ADME, safety, and translational PK variables.
2. Explores variable distributions and pairwise relationships relevant to exposure, clearance, permeability, safety, and tumor coverage.
3. Identifies translational archetypes using principal component analysis and clustering.
4. Trains classification models to predict high developability.
5. Trains regression models to predict projected human clearance and oral bioavailability.
6. Uses model interpretation to identify influential features.
7. Produces a multi-objective rank score for candidate selection.
8. Simulates a simplified PK/PD profile for the top-ranked candidate.

## Main outputs
Produces:
- Summary statistics for the simulated workflow.
- Visualisations of clearance, bioavailability, solubility, lipophilicity, tumor distribution, and coverage.
- Cluster maps and developability landscapes.
- Classification and regression performance metrics.
- Feature-importance plots.
- Ranked candidate tables.
- A simplified PK/PD exposure-versus-potency scenario.

## Intended audience
This project is intended for:
- Translational pharmacology and DMPK scientists.
- Drug discovery scientists working in oncology.
- Hiring managers evaluating quantitative pharmacology and modelling capability.
- Researchers interested in integrating machine learning with mechanistic DMPK reasoning.

## Important note
All data in this repository are simulated for proof-of-concept purposes. The ranges were chosen to be broadly consistent with common DMPK practice and peer-reviewed literature, but the dataset does not represent experimental measurements for real compounds. The outputs should therefore be interpreted as an educational and demonstration, not as a validated preclinical or clinical decision tool.

## How to use
Open notebook to inspect the full analysis and figures. The markdown files provide context on the dataset, model assumptions, limitations, and recommended interpretation.

## Reproducibility
The workflow was designed as a self-contained demonstration. Reproducibility depends on the Python environment, package versions, and random seed settings included in the notebook.

## Citation
**Petalcorin, M.I.R.** (2026). A Molecularly Informed Synthetic Genomics Pipeline for Variant Prioritization, Rare-Variant Burden Testing, Fine-Mapping, and Patient Stratification. https://github.com/mpetalcorin/translational-oncology-dmpk-workflow/edit
If referencing this project, cite it as a simulated proof-of-concept workflow for translational oncology DMPK, machine learning-assisted developability assessment, and candidate selection.
