# Heart-disease-prediction

# Heart Disease Prediction Using ECG

This repository contains the implementation, analysis, and results of the project **"Heart Disease Prediction Using ECG"**, developed under the **Embedded Prototype – 22SDEC14A** initiative at the Department of Electronics and Communication Engineering, Koneru Lakshmaiah Education Foundation.

## 🧠 Project Overview

Heart disease remains a leading cause of death globally. Early detection through predictive analytics can significantly improve patient outcomes. This project leverages **machine learning algorithms** to predict the presence of heart disease based on clinical features derived from ECG and related parameters.

Using the **Cleveland Heart Disease dataset** from the UCI Machine Learning Repository, we trained and evaluated various supervised learning models to identify at-risk individuals with high accuracy.

## 🩺 Key Features

- Supervised learning for binary heart disease classification.
- Ensemble and neural network models trained using **MATLAB’s Classification Learner App**.
- Performance evaluation using **5-fold cross-validation**.
- High validation accuracy (up to **99.2%** using Subspace KNN).

## 🗂️ Dataset Information

**Dataset Source:** UCI Machine Learning Repository – Cleveland Heart Disease dataset  
**Samples:** 303 patient records  
**Features:** 14 clinical attributes including:

- Age, Sex
- Chest pain type (cp)
- Resting blood pressure (trestbps)
- Serum cholesterol (chol)
- Fasting blood sugar (fbs)
- Maximum heart rate (thalach)
- ST depression (oldpeak)
- Thalassemia (thal)
- Target (0 = no disease, 1 = disease)

## 🧪 Methodology

1. **Data Preprocessing**
   - Handled missing values
   - Encoded categorical features
   - Scaled continuous variables
   - Train-test split

2. **Model Training**
   - Models: Logistic Regression, Decision Tree, Random Forest, SVM, KNN, Naive Bayes, Neural Networks
   - Tool: MATLAB Classification Learner App
   - Validation: 5-fold cross-validation

3. **Model Evaluation**
   - Metrics: Accuracy, Precision, Recall, F1-score, Confusion Matrix, ROC-AUC
   - Compared all models and selected the best performing one

## ⚙️ Experimental Setup

- **Tool Used:** MATLAB Classification Learner
- **Dataset Format:** CSV
- **Features Used:** All (140/140)
- **Top Algorithms:**

| Model Type      | Variant                | Accuracy (%) |
|------------------|-------------------------|---------------|
| Ensemble         | Subspace KNN            | 99.2%         |
| Neural Network   | Narrow Neural Network   | 98.8%         |
| Ensemble         | Boosted Trees           | 98.7%         |
| Ensemble         | Bagged Trees            | 98.7%         |
| Neural Network   | Wide/Bilayered          | 98.7%         |

> ✅ **Best model:** Subspace KNN (Ensemble) with **99.2% accuracy**

## 📈 Results

- Ensemble methods consistently outperformed individual classifiers.
- Subspace KNN combined feature space reduction with local decision boundaries.
- Neural networks also showed strong, consistent performance across variants.

## 🔍 Observations

- Ensemble and neural architectures are highly effective for this dataset.
- Preprocessing and feature selection significantly impacted model accuracy.
- Small improvements in validation accuracy can have large impacts in clinical applications.

## 📚 References

- UCI Machine Learning Repository – Cleveland Dataset  
- MATLAB Documentation – Classification Learner App  
- WHO Report – Global Heart Disease Statistics  

## 👥 Authors

- **Balla Pritam** – 2210040026  
- **Kondiparthi Abhilash** – 22100400142  
*Under the guidance of Dr. Ravi Boda*

## 🏁 Future Enhancements

- Apply **PCA** or other feature selection for dimensionality reduction.
- Integrate **Explainable AI** tools (e.g., SHAP, LIME) for model interpretability.
- Deploy as a **real-time diagnostic application** or integrate with **IoT-based ECG monitors**.
- Cross-validate with other clinical datasets to generalize predictions.

---

> 🩺 This project demonstrates the feasibility of using machine learning for early heart disease detection, enabling smarter, data-driven healthcare tools for physicians and patients alike.
