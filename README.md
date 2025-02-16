# 📊 Insurance Premium Prediction

This project aims to predict **insurance premium amounts** based on customer attributes using **machine learning models** such as **XGBoost, LightGBM, CatBoost, and Ridge Regression**. The dataset contains various **demographic, financial, and behavioral features** influencing premium pricing.

---

## 📌 **Project Overview**
- **Objective**: Build a predictive model for insurance premium amounts.
- **Tech Stack**: Python, Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn, XGBoost, LightGBM, CatBoost.
- **Approach**:
  - Exploratory Data Analysis (EDA)
  - Feature Engineering & Encoding
  - Model Training & Cross-Validation
  - Performance Evaluation & Feature Importance Analysis

---

## 📂 **Dataset Description**
The dataset [`train.csv`](https://www.kaggle.com/competitions/playground-series-s4e12/data) consists of **numerical** and **categorical** features influencing insurance premiums.


### **Numerical Features**
| **Feature** | **Description** |
|------------|----------------|
| `Age (Float)` | Customer’s age. |
| `Annual Income (Float)` | Earnings per year. |
| `Health Score (Float)` | Health risk indicator. |
| `Previous Claims (Float)` | Number of past claims. |
| `Vehicle Age (Float)` | Age of insured vehicle. |
| `Credit Score (Float)` | Financial risk measure. |
| `Insurance Duration (Float)` | Policy period. |

### **Categorical Features**
| **Feature** | **Categories** |
|------------|--------------|
| `Gender` | Male/Female |
| `Marital Status` | Single/Married/Other |
| `Education Level` | High School, Bachelor’s, Master’s, etc. |
| `Occupation` | Job type (with significant missing values) |
| `Smoking Status` | Yes/No |
| `Exercise Frequency` | Regular, Occasional, None |
| `Property Type` | Owned, Rented |

### **Target Variable**
| **Feature** | **Description** |
|------------|----------------|
| `Premium Amount (Float)` | The insurance premium charged by the insurer. |

---

## 📊 **Exploratory Data Analysis (EDA)**
- **Distribution Analysis**: Examined the skewness of `Premium Amount`.
- **Correlation Analysis**: Identified weak correlations between numerical features.
- **ANOVA Test**: Found no significant relationships between categorical & numerical features.
- **Missing Values**:
  - **High Missingness**: `Previous Claims` (30%), `Occupation` (29%)


---

## 🔧 **Feature Engineering**
- **Date Features**: Extracted `year`, `month`, `day`, `day of week` from `Policy Start Date`.

---

## 🤖 **Machine Learning Models**
### ✅ **Models Used**: **XGBoost** 🚀
- Tree-based gradient boosting model.
- Used `enable_categorical=True` for native categorical handling.

---

## 🔍 **Model Evaluation**
**Cross-Validation Strategy**: 5-Fold **KFold**  
**Metric Used**: **Root Mean Squared Log Error (RMSLE)**  

| Model | RMSLE |
|--------|------|
| **XGBoost** | `1.04564` |

---

## 📌 **Feature Importance Analysis**
The **top 7 most important features** in **predicting premium amounts**:
1. **Previous Claims** 📈
2. **Customer Feedback** 💬
3. **Annual Income** 💰
4. **Credit Score** 🔢
5. **Year** 
6. **Health Score** ❤️
7. **Marital Status** 💍

---

## 🚀 Future Work
- Hyperparameter Tuning for better performance
- Explainability using SHAP values for better insights.
- Deploying the Model via Streamlit.

## 📬 Contact
For further inquiries or collaboration, please contact me at [tungvu.telecom@gmail.com](mailto:tungvutelecom@gmail.com).
