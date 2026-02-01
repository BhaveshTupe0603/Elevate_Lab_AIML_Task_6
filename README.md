# 🏡 Task 6: Linear Regression

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit_Learn-orange?logo=scikit-learn)

## 📖 Overview
**Task 6** completes the internship technical track by introducing **Regression**. We predicted California housing prices based on census data.

## ⚙️ Workflow
1.  **Data Loading:** Loaded `california_housing` dataset.
2.  **Split:** Divided data into Training (80%) and Testing (20%) sets.
3.  **Modeling:** Implemented **Linear Regression**.
4.  **Evaluation:** Used **MAE** and **RMSE** to measure prediction accuracy.
5.  **Visualization:** Plotted Feature Coefficients to understand *why* the model made its predictions.

## 📊 Key Insights
* **Primary Driver:** Median Income (`MedInc`) is by far the strongest predictor of house value.
* **Model Accuracy:** The model predicts prices with an average error (MAE) of roughly **$53,000**.
<img width="841" height="547" alt="image" src="https://github.com/user-attachments/assets/a1780733-2e11-4889-a417-e800c1d72a98" />
---
# 🏁 Final Outcome: Task 6

## 📊 Evaluation Report
We evaluated the Linear Regression model using standard regression metrics. The target variable (`MedHouseVal`) is scaled in units of **$100,000**.

| Metric | Value | Interpretation |
| :--- | :--- | :--- |
| **MAE** | **0.53** | On average, predictions are off by **$53,000**. |
| **RMSE** | **0.74** | Larger errors (outliers) push this metric higher to **$74,000**. |

## 📉 Predicted vs Actual Analysis
The scatter plot (saved as `predicted_vs_actual_plot.png`) visualizes the model's performance:
* **Alignment:** Most points cluster around the red dashed line (perfect prediction), indicating a strong positive correlation.
* **Deviation:** We see greater spread at higher price points (>$400k), suggesting the model struggles to accurately predict very expensive luxury homes with simple linear features.
* **Cap:** There is a horizontal line of data points at the top ($500k). This indicates the raw dataset "capped" the maximum home value at 500k, causing the model to underestimate these specific homes.

---
## 📂 Deliverables
* [📓 Jupyter Notebook](./Task_6.ipynb)
