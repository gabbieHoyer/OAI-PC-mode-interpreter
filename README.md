# OAI-PC-mode-interpreter 
A MATLAB-based tool for interactive visualization and grading of synthetically generated Principal Component (PC) modes from OAI knee MR images. The app facilitates the interpretation of high-dimensional imaging biomarkers by displaying average 3D joint features along with variations that represent the range observed in patient populations.

This tool is part of the study:  
**Foundations of a Knee Joint Digital Twin from qMRI Biomarkers for Osteoarthritis and Knee Replacement**

For the complementary codebase for the study, see:  
[OAI_digital_twins](https://github.com/gabbieHoyer/OAI_digital_twins)

## Overview
This repository contains code affiliated with the study, “Foundations of a Knee Joint Digital Twin from qMRI Biomarkers for Osteoarthritis and Knee Replacement.” The study forms the basis of a digital twin system of the knee joint, using advanced quantitative MRI (qMRI) and machine learning to advance precision health in osteoarthritis (OA) management and knee replacement (KR) prediction. We combined deep learning-based segmentation of knee joint structures with dimensionality reduction to create an embedded feature space of imaging biomarkers. Through cross-sectional cohort analysis and statistical modeling, we identified specific biomarkers, including variations in cartilage thickness and medial meniscus shape, that are strongly tied to OA incidence and KR outcomes. Integrating these findings into a wide-ranging framework marks a meaningful step toward personalized knee-joint digital twins, potentially strengthening therapeutic strategies and informing clinical decision-making in rheumatological care. This flexible and consistent infrastructure can be adapted to a broad range of clinical approaches in precision health.

## Interactive Visualization and Interpretation
To promote the interpretation of the PCA feature space derived from OAI imaging biomarkers, this MATLAB-based tool provides:
- A visual interface for characterizing structural and compositional tissue changes captured by each PC mode.
- Display of the average 3D representation of a joint feature alongside variations at both extremes, simulating the range observed in the patient population.
- Integration of PCA-derived features with their anatomical context to analyze complex imaging data.
- Support for evaluating the top 10 PC modes for each biomarker, with supplemental tables summarizing mean values and observed variations (mean ± 3 standard deviations) as detailed in the study’s supplementary figures.

This interactive tool serves as a development example of interpretable visualization applications for physicians and researchers.

![app](https://github.com/gabbieHoyer/OAI-PC-mode-interpreter/assets/97639012/9f24ed5b-8555-4e26-83c1-22e0e8a8d040)

# Resources for how to install a MATLAB application
https://www.mathworks.com/help/matlab/ref/appdesigner.html
https://www.mathworks.com/help/compiler/mcr-path-settings-for-run-time-deployment.html

# Local Install and Use 
1. Setup/Export Tab: Choose Output Directory to save interpretations and pc mode images:

![setup_export_tab](https://github.com/gabbieHoyer/OAI-PC-mode-interpreter/assets/97639012/6e90fac7-a689-426e-a547-f487c0e6c70a)

2. Interpretations Tab: 
  a. Choose desired combination of Tissue, Biomarker, and PC Mode.
  b. Use mouse to hover over the pc mode figure and view options to interact with the 3D      pc mode figure.
      1) rotate
      2) pan
      3) maximize/minimize
      4) return to original figure state
  c. View the provided Radiologist interpreation of the 'Upward' (+3 std) and 'Downward'      (-3 std) pc mode. 
  d. Vote in agreement or dissent of the provided interpretations.
     1) if you vote in dissention to the given interpretation, provide your own                 interpretation of the given pc mode. 
  e. Press the 'Save' button to save a screenshot of the workspace.  
  
![interpretation_tab](https://github.com/gabbieHoyer/OAI-PC-mode-interpreter/assets/97639012/fcad5cef-24ee-4570-8c9c-5f6c12386a05)

3. Check List Tab: 
  a. View progress - which PC modes have been evaluated, the provided expert Radiologist interpretation, the vote and interpretation of the user (if applicable).
  b. Filter/Organize the PC mode list by toggling the desired column headers. 
  
![checklist_tab](https://github.com/gabbieHoyer/OAI-PC-mode-interpreter/assets/97639012/3dde272b-11a5-4005-a88a-6afc8efa4af4)

4. Save workspace for later use, or export a pre-existing workspace in the Setup/Export Tab. 

![export_data](https://github.com/gabbieHoyer/OAI-PC-mode-interpreter/assets/97639012/224277f6-7929-4ef9-afe3-3a3514c03066)


## Authors
Gabrielle Hoyer: [Website](https://gabbiehoyer.github.io/)

## Publication
For more details on this work, please refer to the publication:  
**Foundations of a Knee Joint Digital Twin from qMRI Biomarkers for Osteoarthritis and Knee Replacement**  
[npj Digital Medicine](https://www.nature.com/articles/s41746-025-01507-3)

## Reference

```bibtex
@article{Hoyer2025Foundations,
  title  = {Foundations of a knee joint digital twin from qMRI biomarkers for osteoarthritis and knee replacement},
  author = {Hoyer, Gabrielle and Gao, K.T. and Gassert, F.G. and Luitjens, J. and Jiang, F. and Majumdar, S. and Pedoia, V.},
  journal = {npj Digit. Med.},
  volume = {8},
  number = {1},
  pages  = {1--15},
  year   = {2025},
  doi    = {10.1038/s41746-025-01507-3}
}
