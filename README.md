# 🛠️ ML-Powered Predictive Maintenance System

A machine learning-based system to predict potential machine failures using sensor data, enabling proactive and smarter maintenance in industrial environments.

---

## 📌 Problem Statement

Unexpected machine failures in manufacturing can cause costly downtimes and safety risks. This project builds a predictive model that uses real-time telemetry and sensor readings to **anticipate machine failures**, helping industries optimize maintenance schedules and reduce operational disruptions.

---

## 📊 Dataset Overview

The dataset includes sensor measurements and operational settings from different machine types.

**Features:**
- `Type`: Machine type (L, M, H)
- `Rotational speed [rpm]`
- `Torque [Nm]`
- `Tool wear [min]`
- `Air temperature [°C]`
- `Process temperature [°C]`
- `Machine failure`: Binary target variable (0 = No Failure, 1 = Failure)

---

## ⚙️ Key Features & Steps

### ✅ Data Preprocessing
- Handled missing values and encoded categorical features.
- Created new features:
  - `temp_diff`: Difference between process and air temperature.
  - `mechanical_power`: Calculated using torque and rotational speed.

### 📊 Exploratory Data Analysis (EDA)
- Distribution plots for machine types, torque, temperatures, and wear.
- Visualized machine failure trends across types and other factors.

### 🤖 Model Building
Trained and evaluated multiple models:
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting
- XGBoost

### ⚖️ Imbalance Handling
- Used `class_weight='balanced'` in models.
- Evaluated models using metrics suited for imbalanced data.

### 📈 Evaluation Metrics
- Classification Report (Precision, Recall, F1)
- ROC-AUC Scores
- Confusion Matrix
- Precision-Recall Curves

---

## 🧠 Outcome

- Identified key predictors of machine failure.
- Achieved high recall and ROC-AUC, making the model useful for early failure detection.

---

## 🛠️ Tech Stack

- **Language**: Python  
- **Libraries**: Pandas, NumPy, scikit-learn, XGBoost, matplotlib, seaborn  

---

## 🚀 Future Scope

- Deploy using Streamlit or Flask
- Real-time monitoring and alerts
- Model explainability using SHAP or LIME

---

## 📂 Project Structure

