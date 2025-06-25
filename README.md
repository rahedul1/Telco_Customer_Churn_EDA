# Telco_Customer_Churn_Exploratory_Data_Analysis-EDA-
 In-depth Exploratory Data Analysis (EDA) on the Telco Customer Churn dataset to uncover key factors behind customer attrition. Includes data cleaning, visualizations, correlation analysis, and actionable business insights.

This repository presents an in-depth Exploratory Data Analysis (EDA) of the **Telco Customer Churn** dataset. The goal is to understand the factors that influence customer churn in a telecommunications company using statistical and visual techniques.

---

## 🧠 What is Customer Churn?

**Customer churn** refers to the loss of clients or subscribers. In this context, it's when a telecom customer stops using the service.

### Why It Matters:
- Churn affects revenue and growth directly.
- Predicting churn enables proactive retention strategies.
- Helps allocate marketing efforts efficiently.

---

## 📁 Dataset Features

Key columns analyzed:

- `CustomerID`: Unique customer identifier
- `Churn`: Target variable (Yes/No)
- `Tenure`: Customer lifespan (months)
- `MonthlyCharges`: Monthly cost
- `TotalCharges`: Total amount billed
- `Contract`: Contract type (Month-to-month, One year, Two year)
- Other features: `SeniorCitizen`, `Partner`, `Dependents`, `InternetService`, `PaymentMethod`, etc.

---

## 🔍 EDA Overview

### 1. Univariate Analysis
- Understand individual variable distributions (e.g., tenure, charges).
- Visuals: Histograms, boxplots, bar charts.

### 2. Bivariate Analysis
- Study the relationship between two variables (e.g., churn vs. tenure).
- Visuals: Countplots, boxplots, violin plots.

### 3. Multivariate Analysis
- Understand interaction between multiple variables (e.g., churn vs. contract type + monthly charges).
- Visuals: Pair plots, heatmaps, scatter plots.

---

## 📈 Key Insights

| Feature          | Insight                                                                 |
|------------------|-------------------------------------------------------------------------|
| `Contract`       | Month-to-month users churn more.                                        |
| `Tenure`         | Shorter tenure = higher churn.                                          |
| `MonthlyCharges` | Higher charges linked to increased churn.                               |
| `TechSupport`    | Lack of technical support → more likely to churn.                       |
| `OnlineSecurity` | Absence correlates with higher churn.                                   |
| `PaymentMethod`  | "Electronic Check" customers show higher churn rates.                   |
| `InternetService`| Fiber optic users are more likely to churn compared to DSL.             |

---

## 📌 Outlier Detection

Outliers are identified using:
- **IQR Method**
- **Boxplots**
- Found outliers mostly in `MonthlyCharges` and `TotalCharges`.

---

## 📊 Correlation Analysis

Correlations with churn (`Churn_binary` encoded):
- `Tenure`: Strong negative correlation.
- `MonthlyCharges`: Positive correlation.
- `TotalCharges`: Slight negative correlation.

---

## 🖥️ Visualizations Included

- Countplots for categorical features vs. churn
- Boxplots for numerical features vs. churn
- Scatter plots for multi-feature exploration
- Correlation heatmaps

---

## 🧪 Statistical Testing

- **t-test** shows a statistically significant difference in tenure between churned and retained customers (p-value ≪ 0.05).

---

## ✅ Business Implications

- Focus on customer engagement during the **first 18 months**.
- Offer **incentives** to high-churn-risk segments (e.g., short-term contracts, high charges).
- Improve **technical support** and **security features**.

---

## 🛠 Tools Used

- Python (Pandas, NumPy)
- Matplotlib, Seaborn for visualization
- Statistical techniques (correlation, t-tests)
- Jupyter Notebook (recommended for running the analysis)

---
