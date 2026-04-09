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

## Day 28 - Learning Transformer

### 🔹 Topics Covered
1. **ColumnTransformer (scikit-learn)**

   * Understood how to apply **different preprocessing techniques to different columns** in a dataset.
   * Learned why it is important when working with **mixed data types (numerical + categorical)**.
   * Explored how it helps in building a **clean and automated preprocessing pipeline**.

2. **One Hot Encoding (Concept + Memory Handling)**

   * Learned how categorical data is converted into **binary (0/1) format**.
   * Understood the difference between:

     * **Sparse representation** → memory efficient (stores only important values)
     * **Dense representation** → easy to read but memory heavy

3. **`sparse=False` vs `sparse_output=False`**

   * Clarified that:

     * `sparse=False` was used in older versions
     * `sparse_output=False` is the **updated parameter in modern scikit-learn**
   * Understood when to prefer dense vs sparse output:

     * Dense → for learning and debugging
     * Sparse → for large-scale real-world datasets

---

### 🔹 How I Learned

* Focused on **conceptual understanding instead of copy-paste code**
* Broke down each topic into:

  * **Why it is used**
  * **How it works internally**
  * **Real-world intuition (memory, efficiency, pipeline usage)**
* Connected topics to practical ML workflows like:

  * Data preprocessing
  * Feature transformation
  * Pipeline building
 

    ## Day 29 - Learning Pipelines concepts

    firstly I have train and test the model without using the pipeline over the titanic datasets.
    secondly I used pipelines and transformer for the training and test the data.
    I have done this by both ways to analyse hoe the pipelines make the easier to handle in the prroduction level.


     ## Day 30 - Learning Transformer and how to apply
    -> applying log normal
    -> Draw QQ plot before and after applying the log normal
    -> Calculate the predicted values
 
    ## Day 31 - Learning box-cox anf yeo johnson
    -> Apply box-cox tranfroamer
    -> comapare values before and after transformer
    -> draw distplot and QQ pplot before and after applying the transformer
 
    ## Day 31 - Encoding  Numerical dataColumns
    -> Equal Width
    -> Equal frequency
    -> binning
 
     ## Day 32 - Encoding - kbindiscretisation
    -> Applytransformer
    -> create 10 bins for age and fare
    -> use quantile
    

    -> Learn log transformer
    -> Reciprogracal transformer
    -> Square transformer
    -> Square root transformer

