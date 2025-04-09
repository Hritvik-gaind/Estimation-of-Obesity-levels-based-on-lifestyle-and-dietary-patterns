# Estimation-of-Obesity-levels-based-on-lifestyle-and-dietary-patterns

## 📘 Project Overview

This project aims to develop machine learning models that can accurately classify individuals' obesity levels based on their **lifestyle habits** and **dietary patterns**. The dataset contains information from **2,111 individuals** across **Mexico, Peru, and Colombia**, with **17 attributes** including demographic features, eating habits, and physical activity levels.

---

## 🧩 Key Features

- **Dataset**: 2,111 instances with 17 attributes  
- **Target Variable**: `NObeyesdad` (7 obesity levels)  
- **Features**: Includes gender, age, height, weight, family history, dietary habits, physical activity, and more  
- **Models Tested**: Logistic Regression, Decision Trees, Random Forest, XGBoost  

---

## ⚙️ Methodology

### 🔧 Data Preprocessing
- Feature engineering (e.g., BMI calculation, activity scores)  
- Label encoding for categorical variables  
- Checked for missing values (none found)

### 📊 Exploratory Data Analysis
- Visualized distributions of key metrics  
- Analyzed obesity patterns by gender and age  
- Examined feature correlations

### 🤖 Model Development
- Implemented both **multi-class** and **binary classification** approaches  
- Compared performance of different algorithms  
- Conducted hyperparameter tuning to optimize accuracy  

---

## 📈 Results

### Multi-class Classification
| Model               | Default Accuracy | Tuned Accuracy |
|--------------------|------------------|----------------|
| Logistic Regression| 68.6%            | -              |
| Decision Tree       | 78.9%            | -              |
| Random Forest       | 79.6%            | 79.4%          |
| XGBoost             | 79.6%            | **82.0%**      |

### Binary Classification
| Model               | Default Accuracy | Tuned Accuracy     |
|--------------------|------------------|--------------------|
| Logistic Regression| 81.8%            | **83.45% (L2)**    |
| Random Forest       | 88.8%            | 88.42%             |
| XGBoost             | 88.18%           | 88.18%             |

---

## 🧠 Key Findings

- **Tree-based models** (Random Forest, XGBoost) outperformed linear models  
- **XGBoost** showed the best performance for multi-class classification after tuning  
- **Random Forest** demonstrated strongest results for binary classification  
- Feature importance analysis revealed key predictors of obesity levels  
