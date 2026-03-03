# Healthcare Cost Modeling & Statistical Inference

## Project Overview

This project investigates the determinants of healthcare expenditure using statistical inference and predictive modeling techniques.

The dataset consists of 2,000 individuals with demographic, behavioral, and clinical variables. The objective is to identify the primary drivers of annual medical cost and evaluate predictive performance across multiple models.

---

## Research Questions

1. Which variables most strongly influence healthcare expenditure?
2. How large is the effect of smoking on medical cost?
3. Which predictive model best captures cost variability?

---

## Statistical Analysis

- Exploratory Data Analysis
- Correlation analysis
- Welch’s t-test (unequal variances)
- Effect size estimation (Cohen’s d)
- Residual diagnostics

### Key Statistical Result

Smoking effect size: **Cohen’s d = 2.48 (extremely large)**  
Smokers vs Non-smokers: p < 0.001

---

## Predictive Modeling

Models evaluated:

- Linear Regression
- Ridge Regression (CV)
- Lasso Regression (CV)
- Random Forest

### Performance (Test Set)

| Model | R² | RMSE |
|--------|------|-------|
| Linear Regression | 0.615 | 1645 |
| RidgeCV | 0.615 | 1645 |
| LassoCV | 0.612 | 1651 |
| Random Forest | 0.560 | 1759 |

Cross-Validation confirms stable generalization:
- CV R² ≈ 0.60 ± 0.03

---

## Main Insight

Smoking status increases expected annual healthcare expenditure by approximately **4,523 units**, making it the dominant cost driver.

The results suggest a primarily additive and approximately linear cost structure.

---

## Tech Stack

- Python
- Pandas
- NumPy
- SciPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## Repository Structure
data/ → dataset
notebooks/ → full analysis notebook
reports/ → final academic report (PDF)

---

## Author

Dionisis Tare  
Statistics Graduate | Aspiring Data Scientist
