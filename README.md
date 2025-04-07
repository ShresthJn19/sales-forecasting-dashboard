# 📈 Retail Sales Forecasting – Time Series Project

Forecasting monthly retail sales using Prophet to support inventory planning and executive reporting. The project combines time series modeling with business impact simulation and dashboard-ready exports for Tableau.

---

## 🎯 Objective

- Forecast monthly sales for a 5-year retail dataset (2018–2022)
- Capture trend and seasonality using Prophet
- Evaluate accuracy using MAE, RMSE, and MAPE
- Simulate inventory cost savings from better demand estimation

---

## 🧾 Dataset

Simulated Walmart-style sales data:
- **Timeframe**: Jan 2018 – Dec 2022
- **Stores**: Boston Central, Austin North, San Diego East
- **Departments**: Groceries, Electronics, Home & Living

Each record represents total monthly sales for a store-department pair.

---

## 🧠 Methodology

### 🔹 Step 1: Exploratory Data Analysis
- Sales trends by store and department
- Monthly seasonality visualized via boxplots
- Clear upward trend and seasonality detected

### 🔹 Step 2: Forecasting with Prophet
- Data aggregated monthly across all stores and depts
- Trained Prophet with yearly seasonality
- Forecasted 12 months ahead

### 🔹 Step 3: Accuracy Evaluation
- Held out 12 months as test set
- Evaluated forecast using:
  - **MAE** (Mean Absolute Error)
  - **RMSE** (Root Mean Squared Error)
  - **MAPE** (Mean Absolute Percentage Error)

### 🔹 Step 4: Business Simulation
- Modeled 12% holding cost savings on monthly forecast error
- Estimated potential inventory cost reduction

---

## 📊 Results

| Metric         | Value (Example)  |
|----------------|------------------|
| MAE            | $51,211.66           |
| RMSE           | $60,337.28          |
| MAPE           | 17.08%            |
| Cost Savings   | ~$73,744.80/year    |

> ✅ Prophet forecasted sales with high stability and captured both trend and seasonality effectively.

---

## 💼 Business Value

- Forecasting helps avoid over/understocking
- Supports smarter budgeting and resource allocation
- Reduces inventory carrying costs
- Builds a scalable forecasting pipeline for retail operations

---

## 👨‍💻 Tools Used

- Python (pandas, matplotlib, seaborn)
- Facebook Prophet
- scikit-learn (error metrics)
