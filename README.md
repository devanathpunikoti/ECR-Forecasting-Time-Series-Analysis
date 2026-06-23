# ECR Revenue Forecasting using Time Series Analysis

## Project Overview
This project focuses on forecasting ECR [Insert Full Name, e.g., Electronic Cash Register] revenue using Time Series Analysis and Machine Learning techniques. By identifying underlying trends, seasonality, and cyclic revenue patterns, this pipeline generates highly accurate forecasts to support strategic business decision-making and financial planning.

---

## Technologies Used
- **Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Modeling & Stats:** Scikit-Learn, Statsmodels
- **Visualization:** Matplotlib, Seaborn

---

## Project Workflow & Engineering Steps
1. **Data Cleaning & Imputation:** Handled missing values and verified consistent time-frequency intervals.
2. **Exploratory Data Analysis (EDA):** Analyzed revenue distributions and anomalous variance.
3. **Seasonal Decomposition:** Utilized STL/Classical decomposition to isolate underlying trend, seasonal, and residual components.
4. **Time-Series Feature Engineering:** Created lag variables, rolling window statistics (mean, std), and calendar-based features to allow tree-based algorithms to capture temporal dependencies.
5. **Model Training & Evaluation:** Implemented walk-forward validation to train and evaluate models without data leakage.

---

## Model Performance & Evaluation

Models were evaluated using Mean Absolute Error (MAE), $R^2$ Score, and Mean Absolute Percentage Error (MAPE).

| Model | MAE | $R^2$ Score |
| :--- | :---: | :---: |
| **Gradient Boosting Regressor (Best)** | **3,586,185** | **0.662** |
| Decision Tree Regressor | 4,336,942 | 0.513 |
| Random Forest Regressor | 5,068,861 | 0.371 |

### 🎯 Key Performance Highlight:
* **Best Model Accuracy:** The Gradient Boosting Regressor achieved a **MAPE of 7.62%**, representing a **92.38% forecasting accuracy** on the test dataset.

---

## Key Outcomes
- **Extracted Insights:** Successfully isolated distinct weekly/monthly seasonal patterns influencing revenue behavior.
- **Robust Pipeline:** Built an end-to-end forecasting pipeline utilizing tree-based ensemble models engineered specifically for sequential time-series data.
- **Business Ready:** Generated reliable revenue forecasts capable of mitigating financial planning risks.

---

## Author
**Devanath Punikoti** *Computer Science & AI Undergraduate | Machine Learning Engineer*
