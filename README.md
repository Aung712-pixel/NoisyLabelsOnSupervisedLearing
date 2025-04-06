# The Impact of Noisy Labels on Supervised Learning Performance

This project explores how label noise affects the performance of supervised machine learning models. Using a real-world weather dataset (`weatherAUS.csv`), we simulate label noise and compare the performance of models trained on clean vs noisy data.

## Objective

To investigate how introducing noisy labels into the dataset impacts the accuracy and reliability of machine learning classifiers like Random Forest and XGBoost.

---

## Dataset

- **Source:** [Kaggle - Rain in Australia](https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package)
- **Format:** CSV
- **Target Variable:** `RainTomorrow` (Binary classification: Yes/No)

---

## Project Steps

### 1. Data Cleaning
- Removed columns with excessive missing values
- Handled missing numerical and categorical values appropriately
- Ensured the dataset was ready for modeling

### 2. Exploratory Data Analysis (EDA)
- Visualized rainfall distribution by next-day rain outcome using box plots

### 3. Label Noise Injection
- Introduced noise by randomly flipping a percentage of target labels (`RainTomorrow`)

### 4. Model Training & Evaluation
- **Models Used:**
  - Random Forest
  - XGBoost
- Trained on both clean and noisy labels
- Evaluated using:
  - Accuracy
  - Confusion Matrix
  - Classification Report

### 5. Performance Comparison
- Side-by-side visualization of model accuracy
- Analysis of performance drop due to noise

---

## Key Findings

- **Label noise significantly reduced model accuracy**
- **XGBoost was more robust to noise** compared to Random Forest
- Clean data always resulted in higher and more stable performance

---

## Files

- `notebook.ipynb` — Google Colab notebook with full implementation
- `weatherAUS.csv` — Dataset used (upload it manually or link via Kaggle)
- `README.md` — Project summary (this file)

---

## How to Run

1. Upload `weatherAUS.csv` into your Colab session
2. Open the notebook
3. Run all cells to replicate the experiment

---

## Learnings

This project shows the real-world importance of:
- Data quality (especially labels)
- Model evaluation under imperfect conditions
- Visualization and communication of findings

---

## Author

HTET AUNG KHANT
BTECH [CSE]
Built using: Python, Pandas, Scikit-learn, XGBoost, Seaborn, Matplotlib

---
