

# HR Attrition Analysis Project

This project aims to analyze employee attrition data to identify key factors contributing to employee turnover. The analysis involves data preprocessing, exploratory data analysis (EDA), and predictive modeling to understand and predict attrition trends.

## Project Structure

### 1. Data Loading and Preprocessing

- **Data Loading**: The dataset is loaded and split into independent variables (features) and the dependent variable (attrition status).
- **Data Splitting**: The data is divided into training and testing sets.
- **Preprocessing**:
  - **Imputation**: Missing values in numerical features are imputed using the median, and categorical features are imputed using the most frequent value.
  - **Outlier Treatment**: Outliers are clipped to reduce their impact.
  - **Scaling**: Numerical features are scaled for uniformity.
  - **Encoding**: Categorical features are encoded using one-hot encoding.

### 2. Exploratory Data Analysis (EDA)

- **Univariate Analysis**:
  - Distribution of individual features.
  - Attrition rates across different categories.
- **Bivariate Analysis**:
  - Count plots to visualize categorical features against attrition.
  - Box plots, violin plots, scatter plots, and distribution plots for numerical features against attrition.
- **Multivariate Analysis**:
  - Dimensionality reduction and feature importance to understand relationships between multiple variables.

### 3. Model Building and Evaluation

- **Pipeline Construction**: A machine learning pipeline is constructed using the following steps:
  - Preprocessing (as described above).
  - Synthetic Minority Over-sampling Technique (SMOTE) for handling class imbalance.
  - Random Forest classifier for prediction.
- **Model Training**: The pipeline is trained on the training data.
- **Model Evaluation**:
  - Predictions are made on the test data.
  - The model is evaluated using classification metrics such as classification report and accuracy score.

### 4. Results

- The analysis provides insights into the factors influencing employee attrition.
- The predictive model helps in forecasting potential attrition, aiding in proactive retention strategies.
- The `XGBClassifier` (Extreme Gradient Boosting) model demonstrates superior performance in terms of accuracy, weighted average of F1 score, precision, and recall compared to other algorithms tested. This indicates its effectiveness in handling the attrition prediction problem.

## Usage

To run this project:

1. Clone the repository.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Run the Jupyter notebook to see the analysis and results.

## Conclusion

This project provides a comprehensive analysis of HR attrition, combining data preprocessing, exploratory analysis, and predictive modeling to understand and mitigate employee turnover. The `XGBClassifier` has proven to be particularly effective in predicting attrition, making it a valuable tool for HR analytics.

---

Feel free to modify further based on any additional specific insights or findings from your analysis. If you need further customization or more detailed content, let me know!
