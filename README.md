# Titanic Survival Prediction

## Project Overview
This project predicts which passengers survived the Titanic shipwreck using machine learning techniques. It uses the famous Titanic dataset from Kaggle and implements a Random Forest classifier to make predictions.

## Dataset
The Titanic dataset contains information about passengers including:
- Demographics (age, sex, class)
- Ticket information (fare, cabin, embarkation point)
- Family relationships (siblings/spouses, parents/children)
- Survival status (target variable)

## Data Preprocessing
- Handling missing values:
  - Age: filled with median value
  - Fare: filled with median value
  - Embarked: filled with mode
  - Cabin: removed due to excessive missing data
- Feature engineering:
  - Extracted titles from passenger names
  - Created family size feature (SibSp + Parch + 1)
  - Log-transformed fare to handle skewness
- Encoding categorical variables:
  - Sex: converted to binary (0 for male, 1 for female)
  - Embarked: one-hot encoded

## Model
Random Forest Classifier with 100 trees

## Performance
Achieved 82.68% accuracy on the validation set

## Output
Generates a submission.csv file ready for Kaggle submission

## Usage
1. Run the notebook in a Kaggle environment or locally with the required datasets
2. The final output will be a submission.csv file with passenger IDs and survival predictions

## Dependencies
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn 
