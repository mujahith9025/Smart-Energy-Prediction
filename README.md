# ⚡ Smart Energy Consumption Prediction
### A Simple Machine Learning Project | Data Science Course

---

## 📌 Project Overview

This project builds a **Machine Learning model** to predict household energy consumption (in kWh)
based on environmental and usage factors like temperature, number of occupants, and appliances in use.

---

## 🎯 Problem Statement

> *Can we predict how much energy a household will consume given current conditions?*

Predicting energy consumption helps:
- Reduce electricity bills
- Plan energy usage efficiently
- Contribute to sustainability goals

---

## 📊 Dataset Description

**File:** `energy_data.csv`  
**Rows:** 108 records | **Columns:** 8

| Feature | Description | Type |
|---|---|---|
| `Temperature` | Outside temperature in °C | Numeric |
| `Humidity` | Relative humidity (%) | Numeric |
| `Hour` | Hour of the day (0–23) | Numeric |
| `Day_of_Week` | Day (1=Mon … 7=Sun) | Numeric |
| `Month` | Month of the year (1–12) | Numeric |
| `Occupants` | Number of people at home | Numeric |
| `Appliances_On` | Number of appliances switched on | Numeric |
| `Energy_Consumption_kWh` | **TARGET** — Energy used in kWh | Numeric |

---

## 🤖 Machine Learning Models Used

| Model | Description |
|---|---|
| **Linear Regression** | Finds the best straight-line relationship |
| **Decision Tree** | Splits data into decision branches |
| **Random Forest** | Ensemble of many decision trees (best performer) |

---

## 📈 Evaluation Metrics

| Metric | Meaning | Goal |
|---|---|---|
| **MAE** | Mean Absolute Error | Lower is better |
| **RMSE** | Root Mean Squared Error | Lower is better |
| **R² Score** | Explains variance (0–1) | Higher is better |

---

## 🗂️ Project Structure

```
smart-energy-prediction/
│
├── energy_data.csv          ← Dataset
├── energy_prediction.py     ← Main ML script
├── requirements.txt         ← Python dependencies
├── README.md                ← Project documentation
│
├── 01_data_exploration.png  ← Data visualization charts
├── 02_model_comparison.png  ← Actual vs Predicted plots
├── 03_metrics_comparison.png← Model performance bar charts
└── 04_feature_importance.png← Feature importance (Random Forest)
```

---

## 🚀 How to Run

### 1. Install Dependencies
```bash
py -m pip install -r requirements.txt
```

### 2. Run the Project
```bash
py energy_prediction.py
```

---

## 🔄 Project Workflow

```
Load Data → Explore Data → Visualize → Prepare Features
    → Split (80/20) → Scale → Train Models → Evaluate → Predict
```

### Steps Explained:
1. **Load Dataset** — Read CSV into a pandas DataFrame
2. **Explore** — Check shape, types, statistics, missing values
3. **Visualize** — Plot distributions, correlations, trends
4. **Prepare Features** — Select X (inputs) and y (target)
5. **Split Data** — 80% training, 20% testing
6. **Scale Features** — Normalize using StandardScaler
7. **Train Models** — Fit 3 ML models
8. **Evaluate** — Compare MAE, RMSE, R² Score
9. **Feature Importance** — Understand which features matter most
10. **Predict** — Make a real prediction with sample input

---

## 📦 Libraries Used

| Library | Purpose |
|---|---|
| `pandas` | Data loading and manipulation |
| `numpy` | Numerical operations |
| `matplotlib` | Data visualization |
| `seaborn` | Statistical plots |
| `scikit-learn` | Machine learning models and tools |

---

## 💡 Key Findings

- **Appliances_On** and **Occupants** are the most influential features
- Energy consumption peaks during **evening hours** (6–9 PM)
- **Random Forest** outperforms other models due to its ensemble nature
- Higher **temperature** generally correlates with higher energy usage (AC effect)

---

## 📚 Course Information

- **Subject:** Data Science / Machine Learning
- **Topic:** Regression — Predicting Continuous Values
- **Concepts:** EDA, Feature Engineering, Model Training, Evaluation

---

*Built with ❤️ for Data Science Course*
