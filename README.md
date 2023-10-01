# OAI-PC-mode-interpreter 
A MATLAB-based interpretation tool for visualization and grading of synthetically generated Principle Component modes derived from OAI knee MR images. The user can visualize and interpret modes from the 100D PC space consisting of a variety of tissue-biomarker combinations. 

This open-source app was developed as part of an abstract for ISMRM 2023, ML/AI New Ideas oral presentation. 
https://submissions.mirasmart.com/ISMRM2023/Itinerary/ConferenceMatrixEventDetail.aspx?id=121

# Quantitative MRI Interpretable 100D Feature Space of Knee Osteoarthritis
While the Osteoarthritis Initiative data has been explored in independent studies, to our knowledge, never has such a comprehensive analysis been completed, investigating morphology of femur, patella, tibia, menisci, for biomarkers: cartilage thickness, cartilage T2, bone shape, and meniscus shape. With 4,791 subjects from the OAI, this study utilizes an automatic statistical shape modeling technique to create a 100-D interpretable space of biomarker-tissue PC modes, which can be disseminated using an innovative open-source app. In combination with Image Twin and Clinical Twin analyses, variations in morphology, as well as clinical metadata, were identified as being significantly associated with osteoarthritis incidence. 

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


# Medial and Lateral Meniscus PC modes and expert-interpretations soon to come!
