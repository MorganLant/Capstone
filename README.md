
# OCT Segmentation Correction Pipeline

This repository contains the code for the OCT segmentation correction system developed as part of my Capstone Project. The system allows a user to manually correct a boundary on a single OCT B-scan, with this correction then automatically propagated across adjacent slices using a CNN-based model. The aim is to reduce the effort and time required to fix occasional errors made by existing segmentation models.

## 📂 What’s Included
- Full pipeline implementation in the notebook:  
  `Full_Pipeline_with_CNN_and_Editor.ipynb`  
- Interactive editor for making manual corrections  
- CNN model for boundary correction and propagation  

## ⚙️ Running the Pipeline
The code is written and tested in Google Colab. All the required packages, including `oct-vol`, are installed automatically at the start of the notebook.

### To get started:
1. Open the notebook: `Full_Pipeline_with_CNN_and_Editor.ipynb`  
2. Download the model weights and example OCT data from here:  
   (https://drive.google.com/drive/folders/1TtJX1CDfVdqXhRxAXFUKOgcos4u1WHnI?usp=share_link)  
3. Update the file paths in the notebook for the model weights and data.  
4. Use the interactive editor to apply a correction to a chosen B-scan.  
5. Run the pipeline to propagate this correction across the next slices.  
6. Export the corrected segmentation if desired.

The notebook guides you through each of these steps.

## ✏️ Notes
- The interactive editor runs directly within Colab using Dash — it may take a moment to spin up.  
- The system is intended for small local corrections, not for full re-segmentation.  
- No additional setup is needed outside of the notebook and the provided model and data.
