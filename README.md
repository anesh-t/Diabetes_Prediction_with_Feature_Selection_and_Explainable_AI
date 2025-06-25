
# 🔬 Diabetes Prediction Using Machine Learning and Explainable AI

![License](https://img.shields.io/badge/license-CC%20BY--4.0-blue)
![Status](https://img.shields.io/badge/status-published-green)
![Journal](https://img.shields.io/badge/Journal-Frontiers%20in%20AI-blueviolet)

### 📝 Citation  
**Kaliappan J, Saravana Kumar IJ, Sundaravelan S, Anesh T, Rithik RR, Singh Y, Vera-Garcia DV, Himeur Y, Mansoor W, Atalla S, Srinivasan K (2024)**  
"Analyzing classification and feature selection strategies for diabetes prediction across diverse diabetes datasets"  
*Frontiers in Artificial Intelligence*. 7:1421751.  
[RESEARCH ARTICLE LINK](https://www.frontiersin.org/articles/10.3389/frai.2024.1421751/full)

---

## 📌 Overview

This project explores **feature selection** and **classification strategies** for diabetes prediction using diverse public datasets. It combines traditional ML models with **explainable AI** tools (LIME & SHAP) to enhance trust and interpretability in medical AI systems.

### 🔍 Key Contributions
- Evaluated **filter-based** and **wrapper-based** feature selection techniques.
- Used ensemble ML models: Random Forest, XGBoost, Gradient Boosting, and SVM.
- Applied **stacking ensemble** and **meta-learning** using Logistic Regression.
- Interpreted model decisions using **LIME** and **SHAP**.
- Compared results before and after feature selection across **four real-world datasets**.

---

## 📂 Dataset Summary

| Dataset    | Source                                                                                         | Attributes | Key Features                             |
|------------|------------------------------------------------------------------------------------------------|------------|-------------------------------------------|
| Dataset-1  | [Kaggle 1](https://www.kaggle.com/datasets/tigganeha4/diabetes-dataset-2019)                   | 17         | Age, BMI, Stress, Regular Medicine        |
| Dataset-2  | [Kaggle 2](https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset)           | 8          | HbA1c, Blood Glucose, Hypertension        |
| Dataset-3  | [Kaggle 3](https://www.kaggle.com/datasets/andrewmvd/early-diabetes-classification)            | 16         | Polyuria, Polydipsia, Gender              |
| Dataset-4  | [Kaggle 4](https://www.kaggle.com/datasets/mathchi/diabetes-data-set)                          | 8          | Glucose, Insulin, BMI, Age                |

---

## ⚙️ Methodology

1. **Preprocessing**  
   - Missing value imputation (mean/median).
   - Normalization and transformation.

2. **Feature Selection**  
   - *Filter-Based*: Chi-Square, Fisher Score, Information Gain.  
   - *Wrapper-Based*: RF, XGBoost, SVM, Gradient Boosting.

3. **Classification Models**  
   - Base models: `RandomForest`, `XGBoost`, `GradientBoosting`, `SVM`  
   - Meta-model: `LogisticRegression` (Stacking Ensemble)

4. **Explainable AI**  
   - LIME for local interpretability  
   - SHAP for global feature attribution

---

## 📈 Results

| Dataset    | Classifier            | Accuracy (Full Features) | Accuracy (Selected Features) |
|------------|-----------------------|---------------------------|-------------------------------|
| Dataset-1  | Random Forest          | 94.2%                     | 93.7%                         |
| Dataset-2  | Gradient Boosting      | 93.7%                     | 93.7%                         |
| Dataset-3  | Random Forest          | 99.0%                     | 99.0%                         |
| Dataset-4  | Random Forest          | 98.2%                     | 98.6%                         |

> ✅ Stacking Ensemble achieved best overall results in most cases.  
> 📊 Feature selection helped reduce complexity while preserving accuracy.

---

## 📊 Visuals

- SHAP Summary plots  
- LIME decision explanations  
- Correlation matrices  
- Feature importance bar charts  

Place figures under `/visuals` and notebooks under `/notebooks`.

---


## 💡 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/yourusername/diabetes-ml-prediction
cd diabetes-ml-prediction
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the Jupyter notebooks

```bash
jupyter notebook notebooks/diabetes_analysis.ipynb
```

---

## 📚 References

- 📄 [Frontiers in Artificial Intelligence - Published Paper](https://www.frontiersin.org/articles/10.3389/frai.2024.1421751/full)
- 📊 Datasets:
  - https://www.kaggle.com/datasets/tigganeha4/diabetes-dataset-2019
  - https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset
  - https://www.kaggle.com/datasets/andrewmvd/early-diabetes-classification
  - https://www.kaggle.com/datasets/mathchi/diabetes-data-set

---

## 📜 License

This work is licensed under the **[Creative Commons Attribution 4.0 International (CC BY 4.0)](http://creativecommons.org/licenses/by/4.0/)** License.
