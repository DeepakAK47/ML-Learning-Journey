# My ML Learning Journey 🚀

## About This Repository
This repository contains my day by day 
learning of Machine Learning concepts.

## Day 25 - Normalization & Standardization

### What I Learned:
- Normalization scales data between 0 and 1 using MinMaxScaler
- Standardization scales data around mean=0 and std=1 using StandardScaler
- We only scale X (features) not y (target) because y contains class labels not measurements
- We fit the scaler only on x_train to avoid Data Leakage
- Normalization is best when data has no outliers
- Standardization is best when data has outliers

### Tools Used:
Python, Pandas, Scikit-learn, Seaborn, Matplotlib

### Dataset Used:
Wine Dataset



## Day 26 - Norminal and Ordinal Encoding

### Topics Covered
- Understood the difference between **Nominal** and **Ordinal** categorical data
- Learned **Label Encoding**, **Ordinal Encoding**, and when to use each
- Performed **Train-Test Split** using `sklearn` with `random_state` for reproducibility
- Applied data transformations and converted **NumPy arrays back to DataFrames**
- Practiced basic **Git commands** — `git remote -v`, `git pull`, `git push`

### Key Learnings
- Nominal data → One-Hot Encoding
- Ordinal data → Ordinal Encoding
- Always use `random_state=42` in `train_test_split`
- Always `git pull` before `git push`

## Day 27 - One Hot Encoding

Topics Covered

Understood why raw number assignment fails for categorical data
Learned One-Hot Encoding and how it converts categories into binary columns
Understood the Dummy Variable Trap and how to avoid it using drop_first=True
Learned what Multicollinearity is and why it hurts model interpretability
Detected multicollinearity using df.corr() and VIF scores

Key Learnings

Categorical data with no order → One-Hot Encoding
Always use drop_first=True after one-hot encoding
Correlated input features → Multicollinearity
Check multicollinearity with df.corr() — values near 1 or -1 are a red flag
VIF above 10 → fix it immediately












