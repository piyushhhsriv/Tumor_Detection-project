# Tumor Detection Project

This repository contains a Jupyter Notebook implementing a Tumor Detection classification project using the provided Tumor_Detection.csv dataset. The notebook demonstrates data cleaning, exploratory data analysis (EDA), preprocessing, model training, evaluation, and visualization.

## Dataset
- File: `Tumor_Detection.csv`
- Description: Attributes computed from digitized images of fine needle aspirate (FNA) of breast masses. Each row represents a tumor sample with features such as radius, texture, perimeter, area, smoothness, compactness, concavity, concave points, symmetry and fractal dimension. The target label `diagnosis` is 'M' for malignant and 'B' for benign.

## Objective
Build a supervised machine learning model to classify tumors as malignant or benign, while documenting the complete workflow and findings in a Jupyter Notebook.

## Contents
- `Tumor_Detection_Project.ipynb` — Jupyter Notebook with step-by-step analysis, visualizations, preprocessing, and a Random Forest baseline model.
- `Tumor_Detection.csv` — Dataset (place the file in the repository root if not already present).

## Approach
1. Load the CSV into a pandas DataFrame.
2. Clean the data by removing irrelevant columns (for example `id` and any unnamed index columns) and handle missing values.
3. Perform EDA: label distribution, descriptive statistics, and feature correlation heatmap.
4. Preprocess: encode the diagnosis label (`M` = 1, `B` = 0), standard scale features, and split into train/test sets.
5. Train a Random Forest classifier as a baseline. Evaluate with accuracy, classification report, and confusion matrix.
6. (Optional) Explore feature importance, model tuning, and other classifiers.

## How to run
1. Clone the repository:
```bash
git clone https://github.com/piyushhhsriv/Tumor_Detection-project.git
cd Tumor_Detection-project
```
2. Create a virtual environment and install dependencies (recommended):
```bash
python -m venv venv
source venv/bin/activate  # macOS / Linux
venv\Scripts\activate     # Windows
pip install -r requirements.txt
```
3. Open the notebook in Jupyter and run all cells:
```bash
jupyter notebook Tumor_Detection_Project.ipynb
```

If there's no `requirements.txt`, install the common packages used in the notebook:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Results & Notes
- The notebook contains visualizations (count plots, heatmaps) and reports the baseline Random Forest accuracy and classification metrics. Add additional experiments (cross-validation, hyperparameter tuning, other models) to improve performance.
- Make sure `Tumor_Detection.csv` is in the repo root or update the path in the notebook.

## Contributing
Feel free to open issues or pull requests — suggestions for feature engineering, model improvements, and clearer visualizations are welcome.

## Author

*Piyush Srivastava* | [GitHub](https://github.com/yourprofile)
