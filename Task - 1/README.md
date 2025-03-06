# Titanic Survival Prediction - CodSoft Data Science Internship

## Project Overview
This project aims to predict the survival of Titanic passengers using machine learning techniques. The dataset includes details such as passenger class, age, fare, family size, and embarkation point. A Random Forest classifier is used to train the model.

## Dataset Information
The dataset used in this project is **Titanic-Dataset.csv**, which contains the following columns:
- `PassengerId` - Unique ID for each passenger
- `Survived` - Survival status (0 = No, 1 = Yes)
- `Pclass` - Ticket class (1st, 2nd, 3rd)
- `Name` - Passenger name
- `Sex` - Gender (Male/Female)
- `Age` - Passenger's age
- `SibSp` - Number of siblings/spouses aboard
- `Parch` - Number of parents/children aboard
- `Ticket` - Ticket number
- `Fare` - Fare price
- `Cabin` - Cabin number (if available)
- `Embarked` - Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## Preprocessing Steps
1. **Handling Missing Values**:
   - Missing `Age` values are filled with the median age.
   - Missing `Embarked` values are filled with the most common embarkation point.
   - Dropped columns: `PassengerId`, `Cabin`, `Name`, and `Ticket`.
2. **Feature Encoding**:
   - `Sex` converted to binary (0 = Female, 1 = Male).
   - `Embarked` mapped to numeric values (C = 0, Q = 1, S = 2).
3. **Feature Engineering**:
   - Created a new feature `FamSize` (sum of `SibSp` and `Parch`).
   - Dropped `SibSp` and `Parch` after feature engineering.
4. **Rearranged Columns** for better structure.

## Exploratory Data Analysis (EDA)
Several visualizations were created to analyze the survival distribution:
- Survival rate by `Pclass`, `Sex`, and `Age`.
- Distribution of `Fare` and `Embarked` locations.

## Model Training
- **Algorithm Used**: Random Forest Classifier
- **Splitting Data**: 70% Training, 30% Testing
- **Evaluation Metrics**:
  - Accuracy Score
  - Confusion Matrix
  - Classification Report

## Prediction Function
A function is implemented to take user input and predict survival based on the trained model.

## How to Run the Project
1. Install required libraries:
   ```sh
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
2. Place the dataset file (`Titanic-Dataset.csv`) in the same directory as the script.
3. Run the Python script to train the model and test predictions.

## Output
- Displays survival prediction results based on user input.
- Accuracy and classification report after model evaluation.
- Visualizations showcasing dataset insights.

## Future Improvements
- Hyperparameter tuning for better accuracy.
- Deploying the model using Flask or Streamlit.
- Trying other models like XGBoost or SVM for comparison.

## Author
- **CodSoft Data Science Internship** - Titanic Survival Prediction Project

