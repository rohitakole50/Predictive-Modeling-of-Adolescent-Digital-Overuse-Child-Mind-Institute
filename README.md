# Predictive Modeling of Adolescent Digital Overuse (Child Mind Institute)

This project focuses on predicting problematic internet usage in children and adolescents using wearable sensor data related to physical activity, heart rate, and sleep patterns. The goal is to identify behavioral risk factors early and support timely interventions.

## 📊 Project Overview

The dataset is adapted from the [Child Mind Institute](https://www.kaggle.com/competitions/child-mind-institute-problematic-internet-use) and includes time-series sensor data from wearable devices. Our task was to:

- Perform exploratory data analysis (EDA)
- Engineer relevant features from raw parquet files
- Build and evaluate machine learning models
- Derive actionable insights using interpretability techniques

---

## 🧠 Objective

To develop a machine learning model that can accurately predict the level of problematic internet usage in adolescents based on physiological and behavioral signals.

---

## 📁 Dataset Description

- `train.csv` & `test.csv`: Metadata and target variable
- `*.parquet` files: Sensor time-series data (heart rate, activity level, sleep stages, etc.)
- Target variable: **Problematic Internet Use score** (continuous)

---

## 🧪 Techniques Used

- **Time-Series Feature Engineering**: Statistical and rolling-window features from wearable data
- **Data Balancing**: SMOTE for handling target imbalance
- **Modeling**: XGBoost, Random Forest
- **Evaluation**: R² Score, Cross-Validation
- **Explainability**: SHAP for feature importance
- **Visualization**: Multivariate plots, heatmaps, and distributions

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/adolescent-digital-overuse.git
   cd adolescent-digital-overuse
2. Install dependencies
   ```bash
   pip install -r requirements.txt
3. Run notebooks
- Start with EDA_FeatureEngineering.ipynb
- Proceed to Final_Modeling.ipynb for training and evaluation

---

## 📈 Results
- Best model: XGBoost Regressor
- Test R²: 0.72
- Key predictors: Sedentary time, irregular sleep patterns, heart rate variability
- SMOTE application reduced overfitting and improved fairness

---

💡 Key Insights
- Adolescents with lower physical activity and irregular sleep patterns showed higher risk of digital overuse.
- Feature importance analysis via SHAP helped inform potential intervention strategies for behavioral health monitoring.
