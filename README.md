# Cognifyz Task 1 - Predict Restaurant Ratings

## Student Name
Asmit Mohapatra

## Project Title
Predict Restaurant Ratings Using Machine Learning

## Organization
Cognifyz Technologies

## Objective
The objective of this project is to build a machine learning model that predicts restaurant ratings using various restaurant-related features.

## Dataset
The project uses the Zomato restaurant dataset (`dataset1.csv`).

Original dataset size:
- Rows: 9,551
- Columns: 21

## Data Preprocessing
The following preprocessing steps were performed:

- Inspected the dataset structure and column information.
- Checked and handled missing values.
- Filled missing values in the `Cuisines` column with `Unknown`.
- Checked for duplicate records.
- No duplicate records were found.
- Removed restaurants with an `Aggregate rating` of 0 because these records represent restaurants without an actual rating.
- After cleaning, 7,403 records remained.
- Categorical variables were converted into numerical form using One-Hot Encoding.
- The dataset was divided into 80% training data and 20% testing data.

## Features Used

The following features were used for prediction:

- Has Table booking
- Has Online delivery
- Is delivering now
- Price range
- Average Cost for two
- Votes
- City
- Cuisines

## Target Variable

`Aggregate rating`

## Machine Learning Algorithm

Random Forest Regression was used to predict restaurant ratings.

## Model Evaluation

The model was evaluated using the following metrics:

- Mean Squared Error (MSE): 0.1213
- Root Mean Squared Error (RMSE): 0.3483
- R-squared (R2): 0.6078

## Feature Importance

Permutation importance was used to analyze the influence of the selected features on the model's predictions.

The most influential feature identified by the model was:

`Votes`

## Visualizations

The project includes:

1. Actual vs Predicted Restaurant Ratings
2. Feature Importance for Restaurant Ratings

## Tools and Technologies

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Project Files


Task 1 - Predict Restaurant Ratings/
│
├── dataset1.csv
├── Task_1_Restaurant_Ratings.ipynb
└── README.md
