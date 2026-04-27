# Brain Activity Monitoring using AI and Predictive Analysis

## Overview

This project implements EEG classification and event prediction using Machine Learning and Deep Learning models.

The system:

* Preprocesses raw EEG (.edf) data
* Extracts features for ML models
* Trains CNN models for classification and event detection
* Evaluates performance using accuracy, precision, recall, and F1-score

## How to Run

### Option 1 (Recommended – Fast using saved data)

Download and place the following files in your dataset folder:

#### Event Detection Dataset:

* `event_X.npy`
* `event_y.npy`

#### Feature-based ML Dataset:

* `X_train_features.npy`
* `Y_train.npy`
* `X_eval_features.npy`
* `Y_eval.npy`

Then:

1. Update dataset paths in the notebook
2. Run from the **data loading steps onward**


### Option 2 (Full Pipeline – Slow)
1. Download the raw EEG dataset (.edf files)
2. Update dataset paths in the notebook
3. Run all steps from preprocessing

Note:
* Preprocessing is computationally expensive
* May take several hours in Google Colab

## Important Note
All file paths are set for Google Colab (Google Drive).
You **must update paths** based on your environment before running the code.

## Project Structure

* `EEG_classification.ipynb` → ML + CNN classification
* `Event_Detection.ipynb` → Event detection + future prediction
* `README.md` → Instructions
* `requirements.txt` → Dependencies
