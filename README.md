# Linear Regression Analysis on Garment Worker's Productivity

## 📌 Project Overview

This project explores the feasibility of applying a **Linear Regression model** to predict garment workers' productivity. The goal was to determine whether this modeling approach is suitable for the given dataset and to reinforce the importance of validating assumptions before model deployment.

## 📊 Dataset Description

The dataset originates from the **Garment Industry**, a labor-intensive sector critical to global trade. It contains various features related to working teams, departments, work types, target productivity, actual productivity (ranging from 0 to 1), and more.

The main objective was to build a regression model to predict the **actual productivity** of garment workers based on available features.

## 📈 Model Used

- **Linear Regression**

## ⚠️ Key Findings and Takeaways

Despite initial expectations, the Linear Regression model did **not** perform well due to multiple assumption violations:

- **Normality Assumption Violated**:  
  - The p-value from normality tests was **< 0.05**, rejecting the null hypothesis that the data is normally distributed.
  - Histograms of the residuals further confirmed **non-normality**.

- **Linearity & Homoscedasticity Violated**:  
  - The **Residuals vs Fitted** plot showed a **random scatter**, indicating that the relationship between predictors and the target variable is **non-linear** and has **non-constant variance**.

- **Low Model Performance**:  
  - The **R² value was 0.26**, meaning the model explains only **26% of the variability** in worker productivity.
  - Although the **Mean Squared Error (MSE)** was low, the poor R² suggests the model lacks explanatory power.

## 📚 Conclusion

This project is a reminder that:

> ✅ "Not every dataset is suitable for every model."

Applying a Linear Regression model without validating its core assumptions can result in poor and misleading outcomes. Before deploying any model, it is **crucial** to:

- Check the distribution of data
- Evaluate residual plots
- Validate model assumptions such as linearity, normality, and homoscedasticity

In this case, **Linear Regression was not an appropriate fit**, and alternative modeling techniques or data preprocessing steps may be necessary.

## 🛠️ Future Improvements

- Explore **non-linear models** (e.g., Random Forests, Gradient Boosting)
- Perform **feature engineering** or transformation
- Apply **classification techniques** by binning productivity ranges

## 📁 Files Included

- `garment_productivity.csv` – Original dataset
- `linear_regression_analysis.ipynb` – Jupyter notebook with EDA, assumption testing, and model results

---

Feel free to fork or contribute to this project to explore better-suited modeling approaches!
