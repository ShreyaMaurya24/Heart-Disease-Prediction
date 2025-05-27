# ❤️ Heart Disease Prediction Using Random Forest (Colab-Based Project)

This project is a machine learning pipeline built to predict the presence of heart disease using a Random Forest Classifier. It is designed to work with ZIP uploads (containing a CSV file), making it convenient for academic demos and Google Colab use.

---

## 🎯 Objective

The main goal of this project is to:
- Automate the process of uploading and extracting data from a ZIP file
- Handle preprocessing and feature engineering
- Build and evaluate a classification model for heart disease prediction
- Visualize key insights and results

This is part of a broader attempt to apply data science in real-world healthcare problems.

---

## 🛠️ Technologies & Libraries Used

| Library         | Purpose                                     |
|----------------|---------------------------------------------|
| `pandas`        | Data manipulation and reading CSV           |
| `numpy`         | Numerical operations                        |
| `matplotlib`    | Data visualization                          |
| `seaborn`       | Enhanced visualizations (like heatmaps)     |
| `scikit-learn`  | ML algorithms, preprocessing, evaluation    |
| `zipfile`, `io`, `os` | For extracting ZIP files programmatically |
| `google.colab`  | For file uploads in Colab                   |

---

## 📁 Dataset Input Format

- A ZIP file containing **1 CSV file**
- The CSV should contain:
  - Patient details like age, sex, cholesterol, etc.
  - A **binary target column** (like `target`, `output`, or `disease`) indicating heart disease presence

---

## 🔄 Workflow Overview

```text
1. Upload ZIP → Extract CSV → Load Data
2. Handle nulls, encode non-numeric columns
3. Detect target column automatically (binary only)
4. Visualize correlation heatmap
5. Train/test split → Scaling → Train model
6. Evaluate with accuracy, classification report, confusion matrix
7. Plot feature importance + prediction comparison
