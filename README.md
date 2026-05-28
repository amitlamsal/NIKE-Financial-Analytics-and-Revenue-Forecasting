# NIKE Financial Analytics & Revenue Forecasting
### Financial Analysis Dashboard + Machine Learning Revenue Prediction | Webster University

[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)](https://github.com/amitlamsal/nike-financial-analytics-revenue-forecasting)
[![Python](https://img.shields.io/badge/RapidMiner-0073C8?style=flat)](https://github.com/amitlamsal/nike-financial-analytics-revenue-forecasting)
[![Excel](https://img.shields.io/badge/Excel-217346?style=flat&logo=microsoftexcel&logoColor=white)](https://github.com/amitlamsal/nike-financial-analytics-revenue-forecasting)
![Status](https://img.shields.io/badge/Status-Complete-1D9E75?style=flat)

---

## Project Overview

This repository combines two complementary analytics projects on NIKE Inc. — a financial performance dashboard built in Power BI and a machine learning revenue forecasting model built in RapidMiner. Together they deliver a complete analytical picture of NIKE's financial health and future revenue trajectory.

| Aspect | Financial Dashboard | Revenue Forecasting |
|---|---|---|
| **Type** | Descriptive Analytics | Predictive Analytics |
| **Tool** | Power BI | RapidMiner |
| **Data Period** | 5 years (2019–2023) | 20 years (2009–2024 quarterly) |
| **Data Source** | Nike.com, SEC.gov | Nike.com, SEC.gov, Federal Reserve, World Bank |
| **Focus** | Financial health visualization | Future revenue prediction |
| **Course** | Data Visualization | Machine Learning for Business |

---

## Part 1 — Financial Analytics Dashboard (Power BI)

### Business Question
How has NIKE Inc. performed financially over the 2019–2023 period and does it demonstrate the financial strength of a market leader?

### Dataset
Financial data sourced from Nike.com and SEC.gov covering:
- **Income Statement:** Revenue, Cost of Sales, Gross Profit, Net Income
- **Balance Sheet:** Total Assets, Total Liabilities, Shareholders Equity

### Dashboard Analysis

**1. Revenue vs Cost of Sales Trend**
Nike's revenue consistently outpaced cost of sales across 2019–2023. A significant dip occurred in Q2 2020 due to COVID-19 but recovered sharply by Q3 2020. By 2023 revenue reached new highs demonstrating operational resilience.

**2. Gross Profit Comparison**
Gross profit grew steadily from $16K million in 2020 to $22K million in 2023 — reflecting improved pricing strategy and cost control.

**3. Liquidity Analysis**
Liquidity spiked in Q3 2020 as a precautionary measure during pandemic uncertainty. Post-2021 liquidity normalized above pre-pandemic levels indicating efficient cash management.

**4. Assets vs Liabilities**
Total assets consistently exceeded total liabilities across all 5 years — peak asset levels in 2021 and 2022 reaching approximately $150K million. Confirms strong financial stability and low insolvency risk.

**5. Net Profit Margin Trend**
Sharp decline to -20% in Q2 2020 due to COVID-19. Swift recovery above 10% from Q3 2020 onwards — stabilizing and trending upward through 2023.

**6. Revenue vs Industry Expectation**
NIKE total revenue of $218.99K million significantly outperformed the industry benchmark of $80.37K million — a 36.7% surplus above expectations confirming market leadership.

### Key Findings

| Metric | Value | Insight |
|---|---|---|
| Total Revenue (5 years) | $218.99K million | 36.7% above industry benchmark |
| Total Gross Profit | $97.45K million | Strong cost management |
| Total Net Income | $22.82K million | 10.4% of total revenues |
| COVID-19 Impact | Q2 2020 margin -20% | Recovered fully by Q3 2020 |
| Asset-to-Liability ratio | Assets > Liabilities all years | Financially stable throughout |

**Financial Analysis Dashboard**

![Financial Analysis Dashboard](Financial%20Analysis%20Dashboard.png)

**Comparison Dashboard**

![Comparison Dashboard](Comparison%20Dashboard.png)
---

## Part 2 — Revenue Forecasting (RapidMiner Machine Learning)

### Business Question
Can we accurately predict NIKE's future quarterly revenue using financial indicators and macroeconomic variables?

### Dataset
20-year quarterly dataset (2009–2024) combining:

| Variable Type | Variables |
|---|---|
| **Financial Attributes** | Revenue, Total Assets, Total Liabilities, Long-Term Debt, CAPEX, Cash on Hand |
| **Macroeconomic Variables** | GDP Growth Rate, Unemployment Rate, Inflation Rate |
| **Competitor Data** | Adidas financial metrics |
| **Data Sources** | Nike.com, SEC.gov, FRED St. Louis, World Bank |

### Models Tested

| Model | R² | RMSE | Absolute Error | Selected |
|---|---|---|---|---|
| Linear Regression | Good | Low | Low | ✅ Selected |
| Decision Tree | Better | Lower | Lower | ❌ |
| Random Forest | Better | Lower | Lower | ❌ |
| KNN | Best | Lowest | Lowest | ❌ |

### Why Linear Regression Was Selected Over KNN

Despite KNN outperforming all models on performance metrics it was not selected for three reasons:

- **Time Series Limitation** — KNN is not suitable for predicting time series data with a global trend
- **Computational Cost** — Model efficiency decreases significantly with large datasets
- **Data Dependency** — KNN accuracy depends heavily on availability and quality of historical data

Linear Regression was selected as the final model for its interpretability, suitability for time series forecasting and consistent performance.

### Model Details

- **Data Split:** 60% training / 40% testing
- **Deployment:** Created a deployment dataset with updated variable values to generate future revenue predictions
- **Tool:** RapidMiner Studio

**RapidMiner Process Design**

![RapidMiner Process Design](RapidMiner_Process_Design.png)

**Model Prediction Result**

![Model Prediction Result](Model_Prediction_Result.png)
---
## Repository Structure

```
nike-financial-analytics-revenue-forecasting/
│
├── 01_Financial_Dashboard/
│   ├── NIKE_Financial_Dashboard.pbix
│   ├── Financial_Analysis_Report.docx
│   ├── Financial_Analysis_Presentation.pptx
│   ├── Dashboard_Page1.png
│   └── Dashboard_Page2.png
│
├── 02_Revenue_Prediction/
│   ├── Revenue_Prediction_RapidMiner.rmp
│   ├── NIKE_Financial_Dataset_20Years.xlsx
│   └── Revenue_Prediction_Presentation.pptx
│
└── README.md
```

---

## Key Takeaways

- NIKE demonstrates exceptional financial resilience — recovering from COVID-19 faster than industry peers
- Revenue consistently outperformed industry benchmarks by 36.7% across the 5-year period
- Assets exceeded liabilities in every year analyzed confirming long-term financial stability
- Linear Regression provides the most reliable and interpretable revenue forecasting model for NIKE's time series data
- Macroeconomic variables (GDP, Unemployment, Inflation) are significant predictors of NIKE revenue alongside internal financial metrics

---

## Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power BI** | Interactive financial dashboard |
| **RapidMiner** | Machine learning models — Linear Regression, Decision Tree, Random Forest, KNN |
| **Excel** | Data preparation and financial dataset — 20-year quarterly data |
| **PowerPoint** | Project presentations for both analyses |

---

## Education Context

| Project | Course | Professor | University |
|---|---|---|---|
| Financial Dashboard | Data Visualization | Prof. Shawn Higginbotham | Webster University |
| Revenue Forecasting | Machine Learning for Business | Prof. Ahmad Rabiu | Webster University |

---

## About the Author

**Amit Lamsal**
MS Business Analytics — Webster University, St. Louis MO


[![LinkedIn](https://img.shields.io/badge/LinkedIn-amitlamsal-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/amitlamsal)
[![Email](https://img.shields.io/badge/Email-amitlamsal72@gmail.com-D14836?style=flat&logo=gmail)](mailto:amitlamsal72@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-amitlamsal-181717?style=flat&logo=github)](https://github.com/amitlamsal)
