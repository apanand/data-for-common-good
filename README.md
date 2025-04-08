# data-for-common-good

This repository hosts all scripts and files used in the UChicago MSADS Capstone Project to create computer vision models for identifying Chicago neighborhood disorder.

### Public Datasets Used on Roboflow
[Dataset Spreadsheet Link](https://uchicagoedu-my.sharepoint.com/:x:/r/personal/cmarasco_uchicago_edu/Documents/DataSet%20TOC.xlsx?d=w27412bf bba724fdfa1a7227800be68a1&csf=1&web=1&e=suXvY6)

---

## Overview

This project focuses on detecting signs of neighborhood disorder, with a key component being **graffiti detection**. By combining publicly available image datasets with additional collected data, we train and evaluate computer vision models that can identify graffiti in photos.

## Notebooks & Scripts

- **Graffiti Model Trained.ipynb**  
  Demonstrates the end-to-end process of training a CNN-based model for graffiti detection. Includes data loading, preprocessing, training, and evaluation.

- **Heatmap_Image_Collection.ipynb**  
  Contains scripts to collect and process images used for generating a neighborhood “heatmap” based on model predictions.

- **Sample_Heatmap.ipynb**  
  Shows a simple approach to visualizing model outputs on a geographical map of Chicago.

- **app.py**  
  An example Flask application (or similar) to deploy the trained model for real-time inference.

- **graffiti_model_weights.pt**  
  The saved model weights from the trained graffiti detection model (PyTorch format).

---
