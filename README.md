# 🏢 Employee Attrition Prediction: A Comparative Machine Learning Study

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Latest-orange.svg)
![Machine Learning](https://img.shields.io/badge/ML-Supervised%20%26%20Unsupervised-green.svg)

## 📌 Project Overview
High employee turnover (Attrition) is a major challenge for modern organizations. This project builds a predictive pipeline to identify employees likely to leave based on 35 distinct features such as **Monthly Income**, **Overtime**, **Job Satisfaction**, and **Work-Life Balance**. 

By comparing multiple models, this project provides a data-driven approach to help HR departments reduce recruitment costs and improve retention strategies.

---

## 📂 Dataset Key Features
The dataset consists of 1,677 employee records with 35 attributes:
- **Target:** `Attrition` (Binary: 0 for Stay, 1 for Leave)
- **Numerical Features:** Age, MonthlyIncome, DistanceFromHome, TotalWorkingYears, etc.
- **Categorical Features:** Department, JobRole, BusinessTravel, OverTime, etc.

---

## 🛠️ Data Pipeline & Preprocessing
To ensure model robustness, the following steps were implemented:
1. **Outlier Detection:** Used **Boxplots** to identify extreme values in salary and tenure.
2. **Missing Value Imputation:** Intentionally introduced 10% null values and resolved them using **Mean/Mode Imputation** via `SimpleImputer`.
3. **Encoding:** Converted categorical text into numeric data using **One-Hot Encoding**.
4. **Feature Scaling:** Applied **StandardScaler** to normalize features like `MonthlyIncome` and `JobLevel` to a standard range.
5. **Correlation Analysis:** Conducted a "Triple Threat" correlation test (**Pearson, Spearman, and Kendall**) to identify non-linear relationships.

---

## 🤖 Models Implemented
### Supervised Learning (Classification)
We compared three different architectures to find the best predictor:
* **K-Nearest Neighbors (KNN):** A distance-based approach.
* **Decision Tree:** A rule-based logic model for transparency.
* **Neural Network (MLP):** A deep learning approach to capture complex patterns.

### Unsupervised Learning (Clustering)
* **K-Means Clustering:** Applied to group employees into distinct personas.
* **PCA (Principal Component Analysis):** Used to reduce dimensionality for 2D visualization of clusters.

---

## 📊 Performance Metrics
The models were evaluated using:
- **Confusion Matrix:** To track False Negatives (Missed Leavers).
- **ROC-AUC Curve:** To measure the model's ability to distinguish between classes.
- **Precision/Recall:** Focused on maximizing the detection of actual leavers.

*Note: The Neural Network generally showed the highest AUC score (~0.85+).*

---

## 🚀 How to Use
1. Clone the repository:
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)


