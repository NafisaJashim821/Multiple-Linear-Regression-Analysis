# 📊 Advertising Dataset - Multiple Linear Regression Analysis

This project uses a **Multiple Linear Regression** model to analyze and predict product sales based on advertising budgets in **TV**, **Radio**, and **Newspaper** mediums using Python.

---

## 📁 Dataset

- **File:** `Advertising.csv`
- **Columns:**
  - `TV` – Amount spent on TV advertising
  - `radio` – Amount spent on radio advertising
  - `newspaper` – Amount spent on newspaper advertising
  - `sales` – Generated sales revenue

---

## 📌 Objective

To understand how different types of advertising impact sales, and to build a regression model that can predict sales using:
- TV advertising budget
- Radio advertising budget
- Newspaper advertising budget

---

## 🧪 Technologies Used

- Python
- Pandas (for data loading and manipulation)
- NumPy (for numerical operations)
- Matplotlib and Seaborn (for data visualization)
- Statsmodels (for regression modeling)

---

## 🧾 Code Overview

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load the dataset
df = pd.read_csv("Advertising.csv")

✅ What Happens in This Code:
numpy, pandas, matplotlib, and seaborn are imported.

The advertising dataset is loaded using pandas.

📈 Model Summary
Using statsmodels, a Multiple Linear Regression is performed:

Dependent Variable: sales

Independent Variables: TV, radio, newspaper

🔍 The model shows:
R-squared = 0.897 → 89.7% of the sales variation is explained by the ad budgets.

TV & Radio ads have strong positive effects on sales.

Newspaper ads show almost no significant effect.

📊 Visualization & Further Steps
You can visualize:

✅ Correlations between variables

✅ Residuals vs fitted values

✅ Coefficients

📌 Example Visualization:
python
Copy
Edit
sns.pairplot(df, x_vars=['TV', 'radio', 'newspaper'], y_vars='sales', kind='reg')
plt.show()
You may also use heatmaps, residual plots, or coefficient bar charts for more insight.

✅ Conclusion
This analysis helps businesses decide where to invest their advertising budget for maximum return on sales.
The findings show:

TV and Radio are the most effective advertising channels.

Newspaper ads have minimal impact and may not be worth the investment.
