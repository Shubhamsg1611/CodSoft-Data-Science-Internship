# Sales Prediction - CodSoft Data Science Internship

## Project Overview
This project focuses on predicting sales based on advertising spending across different media channels (TV, Radio, Newspaper). A **Linear Regression** model is used to analyze how investments in these advertising channels impact sales performance.

## Dataset Information
The dataset used in this project is **advertising.csv**, which contains the following columns:
- `TV` - Advertising budget spent on TV (in thousands of dollars)
- `Radio` - Advertising budget spent on Radio (in thousands of dollars)
- `Newspaper` - Advertising budget spent on Newspaper (in thousands of dollars)
- `Sales` - Sales generated (in thousands of units, target variable)

## Data Visualization
- **Pairplot Analysis**: Visualizing relationships between all variables
- **Scatter Plots**: Understanding correlations between `Sales` and advertising budgets
- **Boxplots**: Checking for outliers in the dataset
- **Heatmap**: Showing correlations between features

## Model Training
- **Algorithm Used**: Linear Regression
- **Splitting Data**: 80% Training, 20% Testing
- **Evaluation Metrics**:
  - Mean Absolute Error (MAE): 1.27
  - Mean Squared Error (MSE): 2.91
  - Root Mean Squared Error (RMSE): 1.71
  - R² Score: 0.91

## Model Performance
The trained model demonstrates a high level of accuracy with an R² Score of **0.91**, indicating strong predictive power.

## How to Run the Project
1. Install required libraries:
   ```sh
   pip install pandas numpy seaborn scikit-learn matplotlib
   ```
2. Place the dataset file (`advertising.csv`) in the same directory as the script.
3. Run the Python script to train the model and predict sales.
4. Enter new advertising budget values to get predicted sales.

## Prediction Function
The project includes a function that allows users to input TV, Radio, and Newspaper budgets to predict expected sales.

## Future Improvements
- Adding more complex models like Polynomial Regression or Random Forest.
- Deploying the model using a web application (Flask/Streamlit).
- Collecting real-time data for better predictions.

## Author
- **CodSoft Data Science Internship** - Sales Prediction Project
