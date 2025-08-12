# 📊 EDA Automation with LLM (Mistral)

## Overview

This project automates the **Exploratory Data Analysis (EDA)** process using:

- **Python (Pandas, Seaborn, Matplotlib)** for statistical summaries & visualizations
- **Ollama** with the **Mistral** LLM for automated insight generation

The goal is to reduce the time spent on repetitive EDA tasks and leverage AI to interpret datasets in a human-readable way.

---

## ✨ Features

- **Automatic Dataset Summary**
  - Descriptive statistics (`.describe()`)
  - Missing values detection
  - Correlation analysis
- **AI-Powered Insights**
  - Uses **Mistral** via **Ollama** to:
    - Highlight patterns and trends
    - Detect anomalies/outliers
    - Suggest preprocessing steps
    - Provide possible business insights

---

## 🛠️ Tech Stack

- **Python**: Data processing & visualization
- **Pandas**: Data manipulation
- **Matplotlib / Seaborn**: Plotting
- **Ollama**: Local LLM execution
- **Mistral**: Large Language Model for insights

---

## 📂 Project Structure

```/plaintext
│── Dataset
│ └── HR-Employee-Attrition.csv # dataset
│── Notebook
| └── automation.ipynb # EDA with LLM code
└── README.md 
```

---

## AI-Generated Insights

The dataset provided contains information about various employees, their characteristics,

1. Key patterns and trends:

- Most of the variables have a normal distribution, but some (like TotalWorkingYears, TrainingTimesLastYear, YearsAtCompany, YearsInCurrentRole, YearsSinceLastPromotion, and YearsWithCurrManager) seem to be skewed towards lower values.
- There are correlations between certain pairs of variables: for example, StockOptionLevel and TotalWorkingYears appear to be positively correlated, as do YearsAtCompany and YearsInCurrentRole.
- Some variables (like TrainingTimesLastYear, WorkLifeBalance, and StockOptionLevel) have a significant number of missing values, which may require imputation during data preprocessing.

2. Outliers or anomalies:

   - There are a few outliers in the dataset, particularly in variables like StockOptionLevel, TotalWorkingYears, YearsAtCompany, and YearsInCurrentRole. These outliers could potentially be due to errors in data collection or represent unique cases that provide valuable insights.
3. Possible next steps for data preprocessing:

   - Handle missing values by imputation (e.g., mean, median, or mode imputation) or using more advanced techniques like multiple imputation by chained equations (MICE).
   - Perform normalization of the data to ensure that all variables contribute equally during modeling and analysis.
   - Remove outliers if they are errors in data collection or if they do not provide valuable insights for your specific analysis.
   - Explore transforming some variables, such as StockOptionLevel, TotalWorkingYears, YearsAtCompany, and YearsInCurrentRole, to better understand their impact on other variables and outcomes.
4. Potential business insights:

   - There seems to be a correlation between tenure at the current company/role and certain factors like StockOptionLevel and WorkLifeBalance. This may suggest that employees who have been with the company for longer tend to receive more stock options and might also enjoy better work-life balance.
   - Employees who have been with their current manager for a longer time seem to have a higher WorkLifeBalance, indicating the positive impact of a good relationship with one's manager on overall job satisfaction.
   - The outliers in certain variables (like StockOptionLevel and TotalWorkingYears) may represent high-performing employees or long-term dedicated employees who could be valuable assets to the company. Investigating these cases further might provide useful insights for employee retention strategies.
