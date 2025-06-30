# 🛠️ Predictive Maintenance Classification using ML

This project was developed for the course **Aprendizagem Computacional (Machine Learning)** (2023)  
**Bachelor in Informatics Engineering and Bachelor in Electrical and Computer Engineering**,  
**Department of Informatics Engineering – University of Coimbra**

---

## 🎯 Objective

The project aims to solve two classification problems using a synthetic predictive maintenance dataset:

- **Binary Classification**: Predict whether a failure will occur (`Failure = 1`, `No Failure = 0`)
- **Multiclass Classification**: Predict the **type of failure**, among:  
  - Power Failure  
  - Tool Wear Failure  
  - Overstrain Failure  
  - Heat Dissipation Failure

---

## 🧠 Dataset

- Source: [Kaggle – Predictive Maintenance Dataset](https://www.kaggle.com/datasets/shivamb/machine-predictive-maintenance-classification)
- 10,000 samples with 14 features (temperatures, torque, rotation, etc.)
- Includes highly imbalanced classes (majority: No Failure)

---

## 🔬 Methodology

1. **Exploratory Data Analysis (EDA)**:  
   - Visualisation with heatmaps, scatter plots, histograms  
   - Identification of outliers and feature correlation  
   - Cleaning inconsistent records

2. **Preprocessing**:  
   - Ordinal encoding of categorical variables  
   - Feature scaling (RobustScaler, StandardScaler)  
   - Resampling (SMOTE, SMOTE-Tomek) to address imbalance

3. **Models Used**:
   - ✅ **Support Vector Machines (SVM)**  
   - ✅ **Neural Networks** (Keras + RandomSearch tuning)  
   - ✅ **Balanced Random Forest** (extra model)

---

## 📊 Results

### Binary Classification
- **Best model**: Balanced Random Forest + SMOTE-Tomek Links  
  - AUC: 98% | F1-Score: 73%
- SVM also achieved solid AUC of 98% with slightly lower recall on failures.

### Multiclass Classification
- Models reused from binary task
- Neural Network showed high AUC on most failure types but struggled with rare classes.

---

## 📂 Files

- `ML_Project.pdf`: Final report with full implementation and analysis
- `2023-AC-MLProject.pdf`: Official project description
- `src/`: Source code in Python (notebooks and/or scripts)

---

## 👨‍🎓 Authors

- **Gonçalo Tavares de Bastos** – 2020238997  
- **Leonardo Cordeiro Gonçalves** – 2020228071  

📅 Submitted: May 2023
