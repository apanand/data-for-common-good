# data-for-common-good

This repository hosts all scripts and files used in the UChicago MSADS Capstone Project to create computer vision models for identifying Chicago neighborhood disorder.

### Roboflow Public Datasets used for training, testing, validation, and testing
[Dataset Spreadsheet Link](https://uchicagoedu-my.sharepoint.com/:x:/r/personal/cmarasco_uchicago_edu/Documents/DataSet%20TOC.xlsx?d=w27412bf bba724fdfa1a7227800be68a1&csf=1&web=1&e=suXvY6)

### API extracted Google Street View images used for training, validation, and testing
[Dataset Spreadsheet Link]

---

## Overview

Through the files included here, you can:
- Train, evaluate, and deploy a machine learning model to detect graffiti
- Analyze road segments for potential signs of neighborhood disorder
- Collect and organize images for heatmap visualization
- Serve prediction results via a simple web application

---

## Files in This Repository

1. **app.py**  
   - An example Flask application to deploy the trained model for real-time inference. We used ours for a Streamlit sample.
   - Including:
     - Uploading images for inference  
     - Returning predictions (e.g., “graffiti” vs. “no graffiti”)  
     - Basic web form or API endpoints  

2. **Heatmap_Image_Collection.ipynb**  
   - A Jupyter Notebook to collect and process images used for generating a neighborhood “heatmap” based on model predictions.
   - Includes:
     - Code for downloading or fetching images from public sources  
     - Preprocessing steps (resizing, normalizing, etc.)  
     - Saving the data in a structured format for future analysis or model training  

3. **Road Segment Classification Modeling.ipynb**  
   - A Jupyter Notebook dedicated to exploring and modeling road segment data.  
   - Contains:
     - Data wrangling: merging or cleaning road-related data  
     - Model training: classifying types of road segments (e.g., identifying conditions indicative of neglect or disorder)  
     - Evaluation metrics: accuracy, precision, recall, etc.  

4. **Graffiti Model Trained.ipynb**  
   - A Jupyter Notebook that demonstrates end-to-end process of training a CNN-based model for graffiti detection. Includes data loading, preprocessing, training, and evaluation.

5. **graffiti_model_weights.py**  
   - A Python script containing the trained model weights for graffiti detection.
   - Pairs with Graffiti Model Trained.ipynb

6. **Sample_Heatmap.ipynb**  
   - Provides an example of how to visualize the model’s predictions on a map.  
   - Contains:
     - Geographic data manipulation (using latitude/longitude)  
     - Code for creating heatmaps   
     - A demonstration of overlaying model inference data (e.g., graffiti detections) onto a city map  

---
