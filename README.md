
# 🏃‍♂️ Body Performance Analytics: Intelligent Fitness Classification
> Leveraging Machine Learning to predict physical fitness levels based on physiological metrics and performance tests.

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)](https://github.com/)

---

## 📖 Executive Summary
Traditional fitness assessments can be subjective. This project builds an **Intelligent Classification System** using a dataset of **13,393 individuals** to categorize fitness into four classes (A, B, C, D) with high precision.

**Key Insight:** Our analysis identified **Flexibility** (Sit and Bend Forward) as the #1 predictor of overall body performance across all age groups.

---

## 🛠️ The Machine Learning Pipeline

### 1. Data Understanding & EDA
* **Dimensions:** 13,393 rows × 12 features.
* **Target:** `class` (Fitness Level: A=Best, D=Worst).
* **Features:** Age, Gender, Body Fat %, Grip Force, Sit-ups, Broad Jump, etc.

### 2. Data Preprocessing
* **Encoding:** Transformed categorical `gender` and `class` labels using `LabelEncoder`.
* **Scaling:** Standardized physiological measurements to ensure model convergence.
* **Cleaning:** Handled outliers and verified data integrity for consistent results.

### 3. Model Architecture & Comparison
We evaluated five different algorithms to ensure the most robust classification:

| Algorithm | Highlights | Best Accuracy |
| :--- | :--- | :--- |
| **Decision Tree** | Optimized `max_depth` for best interpretability | **73.7%** |
| **Neural Network** | Multi-Layer Perceptron (1-2 Hidden Layers) | **71.5%** |
| **SVM** | Tested with Linear and RBF Kernels | **71.8%** |
| **KNN** | Hyperparameter tuned at $k=25$ | **63.3%** |

---

## 📈 Performance Analysis
Our **Neural Network** achieved a **71.58% Test Accuracy** and was validated using **10-Fold Cross-Validation** ($70.81\% \pm 0.40\%$). 

* **Class D (Highest Accuracy):** 86% Precision (The model is excellent at identifying lower fitness levels).
* **Class A (Top Tier):** 75% Precision.

---

## 📁 Project Structure
```text
├── Data/
│   └── bodyPerformance.csv             # Raw Dataset
├── Notebooks/
│   └── final_project_all_models.ipynb  # ML Experiments & Tuning
├── Documentation/
│   └── Body_Performance_Report.pdf     # Presentation & Visuals
└── README.md
```
---

## 👥 The Core Team

<p align="center">
  <br>
  <b>Mostafa Mohamed</b><br>
  <sub>Project Lead & Data Scientist</sub>
  <br><br>
  <b>Mohamed Abdelhalem</b><br>
  <sub>Data Engineer</sub>
  <br><br>
  <b>Mohamed Hosam</b><br>
  <sub>ML Architect</sub>
  <br><br>
  <b>Mostafa Khalifa</b><br>
  <sub>Visualization Specialist</sub>
  <br><br>
  <b>Ahmed Hassan</b><br>
  <sub>QA & Documentation</sub>
</p>

---
