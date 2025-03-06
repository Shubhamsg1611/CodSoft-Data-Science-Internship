# Movies Rating Prediction App - CodSoft Data Science Internship

## Project Overview
This project focuses on predicting IMDb ratings for movies using machine learning techniques. The dataset contains movie details such as genre, director, actors, year, duration, and votes. A Random Forest Regressor model is trained to estimate movie ratings based on these features.

## Dataset Information
The dataset used in this project is **IMDb Movies India.csv**, which contains the following columns:
- `Name` - Movie title
- `Year` - Release year
- `Duration` - Duration of the movie (in minutes)
- `Genre` - Genre category
- `Rating` - IMDb rating (target variable)
- `Votes` - Number of user votes
- `Director` - Movie director
- `Actor 1` - Lead actor
- `Actor 2` - Supporting actor
- `Actor 3` - Supporting actor

## Preprocessing Steps
1. **Handling Missing Values**:
   - Missing values in `Year`, `Duration`, `Rating`, `Votes`, `Genre`, `Director`, and actors were filled with appropriate median, mean, or mode values.
2. **Feature Encoding**:
   - `Genre`, `Director`, and actor names were encoded using Label Encoding.
3. **Cleaning Votes Data**:
   - Votes with "M" and "K" suffixes were converted to numeric format.

## Model Training
- **Algorithm Used**: Random Forest Regressor
- **Splitting Data**: 80% Training, 20% Testing
- **Evaluation Metrics**:
  - Mean Absolute Error (MAE)
  - R² Score

## Model Performance
The trained model achieved:
- **MAE**: A low mean absolute error indicating good accuracy.
- **R² Score**: Measures how well the model explains rating variations.

## How to Run the Project
1. Install required libraries:
   ```sh
   pip install pandas numpy joblib scikit-learn
   ```
2. Place the dataset file (`IMDb Movies India.csv`) in the same directory as the script.
3. Run the Python script to train the model and predict ratings.
4. Enter movie details when prompted to get an IMDb rating prediction.

## Prediction Function
A function is implemented to take user input (movie genre, director, actors, year, duration, and votes) and predict the IMDb rating based on the trained model.

## Future Improvements
- Exploring deep learning models for better accuracy.
- Deploying the model using Flask or Streamlit.
- Collecting more recent data for improved predictions.

## Author
- **CodSoft Data Science Internship** - Movies Rating Prediction Project

