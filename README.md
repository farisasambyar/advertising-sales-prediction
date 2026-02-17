📈 Sales Prediction Based on Advertising Cost (TV, Radio, Newspaper)

This project aims to predict total sales based on advertising budgets spent on TV, Radio, and Newspaper using a Linear Regression model. The objective is to analyze how advertising costs influence sales performance and to build a predictive model.

1️⃣ Dataset
The dataset is loaded from Google Drive and contains the following columns:

- TV – TV advertising budget
- Radio – Radio advertising budget
- Koran – Newspaper advertising budget
- Total Penjualan – Total sales (target variable)

Notes:
The dataset is read using pandas.read_csv()
No missing values were found in any column

2️⃣ Libraries Used
- pandas
- Data loading and data manipulation using DataFrame
- numpy
- Numerical operations and array handling
- scikit-learn
- train_test_split for splitting data
- LinearRegression for building the prediction model
- plotly

3️⃣ Data Preparation

The dataset is inspected using head() to ensure it is loaded correctly
Missing values are checked using:
data.isnull().sum()

Result:
All columns contain complete data and are ready for analysis

4️⃣ Data Visualization

- Scatter plots are used to analyze the relationship between advertising costs and total sales:

- Sales vs TV Advertising

- Sales vs Radio Advertising

- Sales vs Newspaper Advertising

- Visualization details:

- Point size represents advertising cost

- trendline="ols" is used to show linear trends

Helps identify whether higher advertising spending leads to higher sales

5️⃣ Correlation Analysis

- Correlation is calculated using data.corr() to measure the strength of relationships.

- Correlation with Total Sales:

- TV → Strong correlation

- Radio → Moderate correlation

- Newspaper → Weak correlation

Conclusion:
TV advertising has the strongest influence on sales compared to other media.

6️⃣ Feature Selection
Input Features (X):
- TV
- Radio
- Koran
- Target Variable (y):
- Total Penjualan

These features are selected because advertising spending is expected to directly impact sales.

7️⃣ Train-Test Split

The dataset is divided into:
- 80% training data
- 20% testing data

Configuration:
- test_size = 0.2
- random_state = 42 to ensure reproducible results

8️⃣ Model Training

Algorithm used: Linear Regression
The model is trained using training data with .fit()
The model learns a linear relationship between advertising costs and sales

9️⃣ Model Evaluation

Evaluation metric: R-Squared (R²)
Result:
R² ≈ 0.89

Interpretation:
The model explains about 89% of the variance in sales data

This indicates a strong predictive performance

🔮 Sales Prediction Example

Example input (advertising budget):
- TV = 230.1
- Radio = 37.8
- Newspaper = 69.2

Predicted output:
- Total Sales ≈ 20.13

This shows how the trained model can be used to estimate sales for new advertising budgets.

✅ Conclusion
Advertising costs can be used to predict sales using Linear Regression
TV advertising has the strongest impact on sales

The model performs well with a high R² score

This project can serve as a foundation for more advanced predictive models
