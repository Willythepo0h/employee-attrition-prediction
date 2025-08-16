# 🧠 Employee Attrition Prediction – Machine Learning

This folder contains the **machine learning component** of the Employee Attrition Prediction project.  
The goal is to build predictive models that help HR teams **identify employees at risk of leaving** and provide interpretable insights for decision-making.  

---

## 📂 Files
- **Employee_Attrition_Prediction.ipynb** → Main Jupyter Notebook with full ML workflow.  
- **Employee Attrition Prediction.ipynb – Colab.pdf** → Exported version for easy viewing (no setup required).  
- **README.md** → Documentation for this folder.  

---

## 🔄 Workflow
1. **Data Preprocessing**
   - Handled missing values, categorical encoding, and scaling.  
   - Addressed **class imbalance** using two approaches:  
     - SMOTE (Synthetic Minority Oversampling Technique).  
     - `class_weight=balanced` in Logistic Regression.  

2. **Exploratory Data Analysis (EDA)**
   - Identified key drivers of attrition (e.g., overtime, job role, years at company).  
   - Visualized correlations and feature distributions.  

3. **Modeling**
   - Logistic Regression (baseline + with class weights).  
   - Gradient Boosting.  
   - XGBoost.  

4. **Evaluation Metrics**
   - Classification Report (Precision, Recall, F1-score).  
   - Confusion Matrix.  
   - ROC-AUC Score.  

---

## 📊 Findings

### Logistic Regression (with Class Weights, no SMOTE)
- **ROC-AUC:** ~0.80  
- **Strengths:** High interpretability, solid recall for attrition cases (class 1).  
- **Confusion Matrix Insight:** Balanced detection of attrition while keeping false positives manageable.  

---

## ✅ Conclusion
- **Best Model for Business Use:** Logistic Regression with class weights.  
   - Provides a balance between **predictive power** and **explainability**.  

- Ensemble methods (Gradient Boosting, XGBoost) may be explored further but require careful tuning to outperform Logistic Regression.  

