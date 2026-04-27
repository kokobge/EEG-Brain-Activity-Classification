# Brain Activity Monitoring using AI and Predictive Analysis

## Overview

This project implements EEG classification and event prediction using Machine Learning and Deep Learning models.

The system:
- Preprocesses raw EEG (.edf) data  
- Extracts features for ML models  
- Trains CNN models for classification and event detection  
- Evaluates performance using accuracy, precision, recall, and F1-score  

## Dataset Access

Due to large file sizes, the preprocessed datasets are hosted on Google Drive: https://drive.google.com/drive/folders/1UMv_qz_J8lS90n-PZQRBsf6njEmTFhSP?usp=drive_link

This folder includes:

### Event Detection Dataset
- `event_X.npy`  
- `event_y.npy`  

### Feature-based ML Dataset
- `X_train_features.npy`  
- `Y_train.npy`  
- `X_eval_features.npy`  
- `Y_eval.npy`  

### Processed Datasets

- **Processed_EEG_Dataset/**
train/normal/
train/abnormal/
eval/normal/
eval/abnormal/

Each file:
- `*_X.npy` → EEG windows  
- `*_Y.npy` → labels (0 = normal, 1 = abnormal)

- **Processed_Event_Data/**
X_0.npy, y_0.npy
X_1.npy, y_1.npy
...

Each pair:
- `X_i.npy` → EEG windows  
- `y_i.npy` → labels (0 = normal, 1 = micro-event)
##  How to Run

### Option 1 (Recommended – Fast)

1. Download the `.npy` files from the link above  
2. Update dataset paths in the notebook  
3. Run from the **data loading step onward**  


### Option 2 (Full Pipeline – Slow)

1. Download raw EEG dataset (.edf files)  
2. Update dataset paths  
3. Run all preprocessing steps  


## Code Files

This repository includes:

- `EEG_classification.ipynb` → Main notebook with full pipeline and results   
- `EEG_classification.py` → Clean Python version for reproducibility
- `Event_Detection.ipynb` → Main notebook with full pipeline and results
- `Event_Detection.py` → Event detection and future prediction  

The `.ipynb` files contain executed outputs (accuracy, reports, visualisations).  
The `.py` file is provided for script-based execution.


## Important Note

All file paths are configured for **Google Colab (Google Drive)**.

You must update paths based on your local environment before running the code.
