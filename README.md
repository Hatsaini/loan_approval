# Loan Approval Prediction Project 🏦📊

This project involves building and evaluating predictive models for loan approval using a dataset of 20,000 records. The primary goal is to train classification models, specifically Logistic Regression and K-Nearest Neighbors (KNN), to determine whether a loan will be approved or denied.

## Key Tasks

### 1. Data Cleaning and Preprocessing
- **Handling Missing Values:**
  - Remove columns with over 50% missing values.
  - For categorical columns, delete rows with missing values.
  - For numerical columns, impute missing values with the column mean.
- **Handling Categorical Attributes:**
  - Remove columns where all categorical values are unique.
  - Use one-hot encoding to convert categorical values into numerical ones.

### 2. Logistic Regression Model
- **Dataset Splitting:**
  - Target label: `LoanApproved`
  - Features: All other attributes
  - Train-test split: 80% training, 20% testing
- **Model Training and Evaluation:**
  - Train a logistic regression model.
  - Report accuracy and F1-score for both training and testing datasets.
  - Compare performance metrics for training and testing data.
- **Recursive Feature Elimination (RFE):**
  - Identify effective features by visualizing metric changes with eliminated features.
  - Select an optimal number of features balancing performance and feature minimization.
  - Retrain the model with the selected features.

### 3. K-Nearest Neighbors (KNN) Model
- **1-NN Classifier:**
  - Use features selected from RFE.
  - Train a 1-NN classifier and report accuracy and F1-score for training and testing datasets.
  - Compare performance metrics between training and testing data.
- **Grid Search with Cross-Validation:**
  - Perform grid search over `K` values (1-30) with 5-fold cross-validation.
  - Visualize accuracy changes with `K` using a line chart.
  - Report best-case metrics.
- **Distance Metric Analysis:**
  - Test performance with three distance metrics: Euclidean (L2), Manhattan (L1), and Cosine.
  - Visualize results using a bar chart for both accuracy and F1-score.

## Tools and Technologies
- **Languages:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

## Project Highlights
- Comprehensive data cleaning and feature engineering to ensure model readiness.
- Built and evaluated Logistic Regression and KNN models with robust validation techniques.
- Insightful analysis of model performance through visualizations and comparisons.
- Applied advanced techniques like RFE and grid search to optimize models.

Feel free to explore the code, visualizations, and results in the notebook. Feedback and suggestions are always welcome!
