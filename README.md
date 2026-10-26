# My Machine Learning Learning Journey

This repository contains my hands-on, day-by-day exploration of machine
learning. The notebooks move from exploratory data analysis and data
preprocessing to regression, classification, ensemble learning, and
clustering. Most examples use Python, Pandas, NumPy, Matplotlib, Seaborn, and
scikit-learn.

## Repository Structure

The learning material is organised into phase folders:

| Phase | Days | Main focus |
| --- | --- | --- |
| [`fir_sec_phase/`](./fir_sec_phase/) | 18, 20 | Web scraping and exploratory data analysis |
| [`third_phase/`](./third_phase/) | 21–30 | Data analysis, feature transformation, and pipelines |
| [`fourth_phase/`](./fourth_phase/) | 31–40 | Feature engineering and missing-value handling |
| [`fifth_phase/`](./fifth_phase/) | 41–50 | Outliers, PCA, and linear regression |
| [`sixth_phase/`](./sixth_phase/) | 51–60 | Optimisation, regularisation, and classification |
| [`seventh_phase/`](./seventh_phase/) | 61–69 | Decision trees, ensemble learning, and clustering |

The current repository does not contain separate `first_phase` or
`second_phase` folders. The earliest available notebooks are in
[`fir_sec_phase/`](./fir_sec_phase/).

## Learning Roadmap

### First and Second Phase — Foundations

There are no separate folders for these phases in the current repository.
They are represented by the earliest available learning work in
[`fir_sec_phase/`](./fir_sec_phase/).

### First/Second Phase Material — Web Scraping and EDA

Available notebooks: `day18.ipynb`, `day20.ipynb`

- Scrape web pages with `requests` and `BeautifulSoup`
- Convert extracted web data into a Pandas table
- Perform univariate exploratory data analysis
- Analyse categorical variables with count plots and pie charts
- Analyse numerical variables with histograms and box plots

### Third Phase — EDA and Feature Transformation

Available notebooks: days 21–30 in [`third_phase/`](./third_phase/).

- Perform bivariate analysis for numerical and categorical variables
- Use cross-tabulation, heatmaps, cluster maps, and pair plots
- Generate automated exploratory reports
- Split data into training and test sets
- Apply standardisation and min-max normalisation
- Encode ordinal and nominal categorical data
- Apply label encoding, ordinal encoding, and one-hot encoding
- Use `ColumnTransformer` for mixed numerical and categorical data
- Build and compare preprocessing pipelines
- Apply function transformations such as logarithmic transformations
- Visualise distributions and Q-Q plots before and after transformation

### Fourth Phase — Feature Engineering and Missing Data

Available notebooks: days 31–40 in [`fourth_phase/`](./fourth_phase/).

- Transform numerical variables using log, reciprocal, square, and square-root
  transformations
- Apply power transformations such as Box-Cox and Yeo-Johnson
- Discretise numerical features with equal-width and equal-frequency binning
- Use `KBinsDiscretizer` and binarisation
- Handle mixed data types and date-time features
- Remove rows with missing values using complete-case analysis
- Impute numerical values with mean, median, arbitrary, and random-sample
  strategies
- Impute categorical values using the most frequent category or a constant
- Add missing-value indicators and model missingness
- Apply multivariate imputation with `KNNImputer`
- Compare different imputation strategies using model performance

### Fifth Phase — Outliers, PCA, and Linear Regression

Available notebooks: days 41–50 in [`fifth_phase/`](./fifth_phase/).

- Detect and understand outliers
- Remove or cap outliers using Z-scores, box plots, percentiles, and
  Winsorization
- Construct new features and split existing features
- Reduce dimensionality with Principal Component Analysis (PCA)
- Visualise PCA projections in two and three dimensions
- Build simple linear regression models with scikit-learn
- Implement linear regression from scratch
- Add relevant features and evaluate predictions
- Build multiple linear regression models
- Compare implementations from scratch with scikit-learn
- Study linear-regression assumptions:
  - Linearity
  - Multicollinearity
  - Normally distributed residuals
  - Homoscedasticity
  - Autocorrelation

### Sixth Phase — Optimisation, Regularisation, and Classification

Available notebooks: days 51–60 in [`sixth_phase/`](./sixth_phase/).

- Understand ordinary least squares and gradient descent
- Implement batch, stochastic, and mini-batch gradient descent
- Build polynomial regression models
- Use Ridge regression and understand L2 regularisation
- Implement Ridge regression from scratch and with gradient descent
- Use Lasso regression and understand L1 regularisation
- Apply Elastic Net regression
- Understand the perceptron approach to classification
- Build logistic regression models and train them with gradient descent
- Evaluate binary classifiers with ROC curves and AUC
- Apply Softmax logistic regression for multiclass classification
- Extend logistic regression to non-linear data with polynomial features
- Apply K-nearest neighbours (KNN)
- Build support-vector machine (SVM) classifiers

### Seventh Phase — Trees, Ensembles, and Clustering

Available notebooks: days 61–69 in [`seventh_phase/`](./seventh_phase/).

- Build decision-tree classifiers and regressors
- Visualise trees and explain prediction paths with Graphviz and `dtreeviz`
- Apply hard, soft, and weighted voting ensembles
- Use bagging for classification and regression
- Explore pasting, random subspaces, random patches, and out-of-bag scoring
- Tune ensemble models with `GridSearchCV`
- Build and compare random forests with bagging models
- Analyse random-forest feature importance
- Use grid search and random search for hyperparameter tuning
- Implement AdaBoost from scratch and with scikit-learn
- Understand and apply gradient boosting for regression and classification
- Combine models using stacking and blending
- Apply K-means clustering
- Visualise clusters in two and three dimensions

## Tools and Libraries

- Python
- Jupyter Notebook
- NumPy and Pandas
- Matplotlib, Seaborn, and Plotly
- SciPy and Statsmodels
- Scikit-learn
- BeautifulSoup and Requests
- Graphviz and `dtreeviz`
- `mlxtend`
- `ydata-profiling`

## Saved Model Artifacts

The [`models/`](./models/) folder contains serialized preprocessing and model
artifacts:

- `clf.pkl` — trained classifier
- `ohe_embarked.pkl` — encoder for the Embarked feature
- `ohe_sex.pkl` — encoder for the Sex feature

These artifacts support the Titanic classification and preprocessing
experiments explored in the notebooks.

