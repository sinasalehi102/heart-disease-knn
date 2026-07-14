
# KNN Heart Disease Classification

## Overview
KNN classifier on the Heart Disease dataset. Compared performance across different imputation strategies, scaling methods, and k values using 5-fold cross-validation. 

## Results

| Impute | Scale   | Best k | Accuracy | Precision | Recall | F1    |
|--------|---------|--------|----------|-----------|--------|-------|
| mean   | zscore  | 5      | 0.8525   | 0.8421    | 0.8649 | 0.8533 |
| mean   | minmax  | 7      | 0.8361   | 0.8286    | 0.8421 | 0.8353 |
| mean   | robust  | 3      | 0.8197   | 0.8108    | 0.8333 | 0.8219 |
| median | zscore  | 5      | 0.8443   | 0.8378    | 0.8485 | 0.8431 |
| median | minmax  | 9      | 0.8279   | 0.8158    | 0.8421 | 0.8288 |
| median | robust  | 5      | 0.8115   | 0.8000    | 0.8235 | 0.8116 |

See `results/figures/` for full results including elbow plots and confusion matrices.

## Requirements
- pandas
- scikit-learn
- matplotlib
- seaborn

## Usage
Run `notebooks/knn_analysis.ipynb` to reproduce results.
