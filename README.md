# 🛠️ ML-Powered Predictive Maintenance System

A machine learning-based system to predict potential machine failures using sensor data, enabling proactive and smarter maintenance in industrial environments.

---

## 📌 Problem Statement

Unexpected machine failures in manufacturing can cause costly downtimes and safety risks. This project builds a predictive model that uses real-time telemetry and sensor readings to **anticipate machine failures**, helping industries optimize maintenance schedules and reduce operational disruptions.

---

## 📊 Dataset Overview

The dataset includes sensor measurements and operational settings from different machine types.

The dataset used in this project can be accessed [here](https://www.kaggle.com/datasets/stephanmatzka/predictive-maintenance-dataset-ai4i-2020).

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

### ⚖️ Imbalance Handling
- Used SMOTE Technique to handle imbalanced dataset
- Used `class_weight='balanced'` in models.

### 📈 Evaluation Metrics
- Classification Report (Precision, Recall, F1)
- ROC-AUC Scores
- Confusion Matrix
- Precision-Recall Curves

---
## 🛠️ Tech Stack

- **Language**: Python  
- **Libraries**: Pandas, NumPy, scikit-learn, matplotlib, seaborn  

---
## 🧠 Outcome

Achieved a reliable model that can proactively predict machine failures with high precision and recall, significantly improving maintenance planning and operational efficiency.


