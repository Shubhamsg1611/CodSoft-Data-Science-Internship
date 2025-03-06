# Iris Flower Classification - CodSoft Data Science Internship

## Project Overview
This project focuses on classifying Iris flowers into three species (**Iris-setosa, Iris-versicolor, and Iris-virginica**) using machine learning techniques. A **Random Forest Classifier** is trained to predict the species based on sepal and petal measurements.

## Dataset Information
The dataset used is **IRIS.csv**, which contains the following columns:
- `sepal_length` - Length of the sepal (cm)
- `sepal_width` - Width of the sepal (cm)
- `petal_length` - Length of the petal (cm)
- `petal_width` - Width of the petal (cm)
- `species` - Flower species (target variable)

## Data Visualization
- Histograms of sepal and petal dimensions categorized by species.
- Pairplots to analyze relationships between features.
- Heatmap to display feature correlations.

## Model Training
- **Algorithm Used**: Random Forest Classifier
- **Splitting Data**: 80% Training, 20% Testing
- **Evaluation Metrics**:
  - Accuracy Score
  - Classification Report
  - Confusion Matrix

## Model Performance
The trained model achieved:
- **High accuracy**, demonstrating its reliability in classifying Iris species.
- **Confusion matrix visualization** to assess classification errors.

## How to Run the Project
1. Install required libraries:
   ```sh
   pip install pandas numpy seaborn scikit-learn matplotlib
   ```
2. Place the dataset file (`IRIS.csv`) in the same directory as the script.
3. Run the Python script to train the model and classify Iris flowers.
4. Enter flower measurements when prompted to predict the species.

## Prediction Function
A function is implemented to take user input for sepal and petal dimensions and predict the Iris species based on the trained model.

## Future Improvements
- Exploring other classification models for improved accuracy.
- Deploying the model using Flask or Streamlit.
- Expanding the dataset for broader classification use cases.

## Author
- **CodSoft Data Science Internship** - Iris Flower Classification Project
