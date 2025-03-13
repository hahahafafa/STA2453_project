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
├── scripts/
│   ├── overlay_masks.py         # Script for overlaying brain masks on MRI data
│   ├── feature_engineering.py   # Script for feature extraction and engineering
│   └── train_model.py           # Script for training ML/DL models
├── README.md                    # This file
└── requirements.txt             # List of required Python packages
```

---

## How to Use

1. **Exploratory Data Analysis:**  
   - Open the `notebooks/EDA.ipynb` file to explore the MRI data, view distributions, and perform quality checks.

2. **Overlay Masks:**  
   - Use the script in `scripts/overlay_masks.py` to apply the brain mask to the MRI data, reducing background noise and focusing on brain tissue.

3. **Feature Engineering & Modeling:**  
   - Run `scripts/feature_engineering.py` to extract key features from the MRI images.
   - Train your predictive model by running `scripts/train_model.py`.

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
