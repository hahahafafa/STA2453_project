# STA2453_project


This repository contains the code and documentation for a project aimed at predicting patient recovery time using MRI scans and demographic data. The goal is to provide insights into recovery patterns and help inform future clinical decision-making. This project uses both machine learning and deep learning methods to analyze brain images and clinical features.

---

## Repository Structure

```
├── data/
│   ├── cleaned_output.h5        # HDF5 file containing cleaned MRI data
│   └── brain_mask.h5            # HDF5 file containing brain masks
├── notebooks/
│   ├── EDA.ipynb                # Notebook for exploratory data analysis
│   └── PCA_analysis.ipynb       # Notebook for PCA and dimensionality reduction
├── example/                     # Example usage: quick run with pretrained model
├── scripts/
│   ├── overlay_masks.py         # Script for overlaying brain masks on MRI data
│   ├── feature_engineering.py   # Script for feature extraction and engineering
│   └── train_model.py           # Script for training ML/DL models
├── documentation/
│   └── Proposal.pdf             # Proposal of the data
└── README.md                    # This filees
```

---

## How to Use

Perfect — I’ll write a **polished, professional README update** that:

- Shows where your `example/` folder fits
- Explains **how to quickly run** the reproducible example
- Makes your repo very clean and easy for others to navigate!

---

# 📄 Example README Update

## Project Overview
This repository contains code and models for predicting concussion recovery time using 3D brain MRI data and demographic information.  
It includes MRI preprocessing, model training, evaluation, and a lightweight example to quickly demonstrate the workflow without full retraining.

---

## Repository Structure

```bash
├── example/               # Example usage: quick run with pretrained model
├── models/                # CNN model definitions
├── data/                  # Processed datasets (e.g., cleaned_output.csv, brain mask, H5 file)
├── saved_models/          # Pretrained model checkpoints (.pth)
├── notebooks/             # Exploratory data analysis and training notebooks
├── scripts/               # Helper scripts (reconstruction, training, evaluation)
├── original_shape.npy     # Saved original MRI volume shape
├── README.md              # Project documentation
```

---

## Quick Start: Example Usage

You can **run a reproducible example** directly without training the model from scratch.

### 1. Install Requirements

Make sure you have the following packages installed:
```bash
pip install torch numpy pandas matplotlib h5py tqdm seaborn
```

### 2. Run the Example

```bash
cd example
python reproducible_example.py
```

This script will:
- Load sample MRI + demographic data
- Generate predicted recovery times
- Plot predicted vs. actual recovery times

✅You can reproduce the key results in just a few seconds.

---


## Notes
- MRI data volumes were reconstructed using a brain mask and saved in H5 format.
- The target variable is log-transformed recovery time (`log(d_Recov + 1)`).
- Original MRI shape is saved in `original_shape.npy` for reproducibility.

---

## Workflow Overview

- **Data Cleaning:** The raw MRI data and masks are stored in HDF5 files. The code cleans and organizes these data for further analysis.
- **Masking:** The brain mask is applied to each MRI scan to remove non-brain regions.
- **Dimensionality Reduction:** PCA and other methods are used to reduce the high-dimensional MRI data.
- **Model Training:** Both machine learning and deep learning techniques are explored to predict recovery time from the extracted features.
- **Evaluation:** The models are evaluated using various performance metrics to determine the best approach.

---

## Feedback

All feedback is documented in the repository. Feel free to check the `feedback/` folder for details on improvements and future directions.

---

Feel free to clone this repository, explore the notebooks, and run the scripts to reproduce the analysis. If you have any questions or suggestions, please open an issue or contact me directly.

Enjoy exploring the data!
