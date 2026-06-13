# Carseats — Machine Learning Classification & Clustering

**Author:** Malek Jaafra
**Platform:** Kaggle
**Language:** Python

---

## Project Overview

This project applies Machine Learning algorithms on the **Carseats dataset** to:

* Classify stores based on sales performance (High vs Low)
* Cluster stores based on price and regional income patterns

---

## Dataset

* **Source:** Carseats Dataset (Kaggle)
* **Target Variable:** High Sales (Sales > 8 → 1, else → 0)
* **Features:** Price, Income, Advertising, Population, ShelveLoc, Age, and other store characteristics

---

## Project Workflow

### 1. Data Preprocessing

* Target variable creation: `High = (Sales > 8)`
* One-Hot Encoding of categorical variables
* Train/Test split (70% / 30%)
* Feature scaling with StandardScaler

### 2. Supervised Learning — Classification

* **KNN** tested for k = 1, 3, 5, 7, 9
* **Random Forest** (100 estimators)
* **SVM** (RBF kernel)
* Evaluation using:

  * Accuracy Score
  * Classification Report
  * Confusion Matrix
* Feature importance visualization (Top 7 variables)

### 3. Unsupervised Learning — Clustering

* **K-Means** tested for k = 2, 3, 4
* Visualization using Price vs Regional Income scatter plots

---

## Model Results

| Algorithm        | Accuracy |
| ---------------- | -------- |
| KNN (best k = 3) | 76.7%    |
| Random Forest    | 80.0%    |
| SVM (RBF)        | 84.2%    |

**Best Model:** SVM (RBF Kernel) with an accuracy of **84.2%**.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn
* Matplotlib
* Jupyter Notebook

---

## Repository Structure

```text
Carseats-ML-Classification/
├── projet_ml.ipynb
├── Carseats.csv
└── README.md
```

---

## Author

Malek Jaafra
