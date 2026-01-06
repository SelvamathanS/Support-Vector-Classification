# Breast Cancer Diagnosis Prediction using SVM

This project implements a **Support Vector Machine (SVM)** model to classify breast cancer diagnoses as malignant or benign using a structured dataset. The workflow includes data preprocessing, model training, evaluation, and visualization of results.

---

## 📌 Project Overview

The goal of this project is to:

* Load and preprocess a breast cancer dataset
* Train an SVM classifier
* Evaluate model performance using accuracy, classification report, and confusion matrix
* Visualize prediction results

---

## 📂 Dataset

* **File name:** `breast-cancer.csv`
* **Target column:** `diagnosis`
* **Features:** All remaining numerical columns
* The dataset is loaded using **pandas**

> ⚠️ Make sure to update the dataset path if you are not using Google Drive or Colab.

---

## 🧰 Libraries Used

* `pandas`
* `numpy`
* `scikit-learn`
* `matplotlib`

Install required packages (if not already installed):

```bash
pip install pandas numpy scikit-learn matplotlib
```

---

## 🔄 Workflow

### 1. Data Loading

The dataset is loaded into a pandas DataFrame.

### 2. Feature & Target Split

* **X:** All columns except `diagnosis`
* **y:** `diagnosis` column

### 3. Train-Test Split

* 70% training data
* 30% testing data
* `random_state = 42` for reproducibility

### 4. Feature Scaling

* Standardization using `StandardScaler`
* Ensures better SVM performance

### 5. Model Training

* Support Vector Classifier (`SVC`)
* Default kernel and parameters

### 6. Model Evaluation

* Accuracy score
* Classification report (precision, recall, F1-score)
* Confusion matrix visualization

---

## 📊 Results

* **Accuracy** is printed in the console
* **Classification Report** shows detailed metrics
* **Confusion Matrix** visualizes correct vs incorrect predictions

Example output:

```
SVC Model Accuracy: 0.97
```

---

## 📈 Confusion Matrix

The confusion matrix helps understand:

* True Positives
* True Negatives
* False Positives
* False Negatives

It is displayed using `ConfusionMatrixDisplay` from `sklearn`.

---
