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

The dataset provided contains information about various employees, their characteristics, and job details. Here are some insights from the summary:

- Total number of observations (employees) is 1470.
- The mean age of employees is approximately 36.9 years, with a standard deviation of  9.14. This suggests that there's a diverse range of ages in the dataset.
- The average daily rate and hourly rate are around $802.49 and $65.89 respectively.   The mean monthly income is approximately $6502.93.
- Employees work, on average, 11.28 hours per week (StandardHours), with a standard deviation of 3.66 hours. This indicates a wide range in the working hours of employees.
- The mean number of companies worked is 14313.1, suggesting that employees have had multiple job experiences.
