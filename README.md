# Titanic Survival Prediction

## Objective
The objective of this project is to build a predictive model that determines whether a passenger on the Titanic survived or not based on features such as age, gender, class, fare, and more. The dataset contains historical data from the Titanic, and the goal is to predict the likelihood of survival using machine learning techniques.

## Dataset
The dataset used for this project contains the following columns:

- **PassengerId**: Unique ID of each passenger.
- **Survived**: Target variable (0 = No, 1 = Yes).
- **Pclass**: Passenger class (1st = Upper, 2nd = Middle, 3rd = Lower).
- **Name**: Name of the passenger.
- **Sex**: Gender of the passenger (male, female).
- **Age**: Age of the passenger (in years).
- **SibSp**: Number of siblings or spouses aboard the Titanic.
- **Parch**: Number of parents or children aboard the Titanic.
- **Ticket**: Ticket number.
- **Fare**: Amount of money the passenger paid for the ticket.
- **Cabin**: Cabin number (may have missing values).
- **Embarked**: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

## Steps Taken in the Project

1. **Data Preprocessing**:
   - Handle missing values in the dataset.
   - Encode categorical variables (e.g., Sex and Embarked).
   - Normalize and scale data where necessary.

2. **Model Building**:
   - Split the dataset into training and testing sets.
   - Use machine learning algorithms (e.g., Random Forest) to train the model.
   
3. **Model Evaluation**:
   - Evaluate the model performance using metrics like accuracy, precision, recall, and confusion matrix.

4. **Model Improvement**:
   - Experiment with different models and hyperparameter tuning to improve prediction accuracy.

## Handling Missing Data
Some columns, such as Age, Cabin, and Embarked, might have missing values. Here's how the missing data was handled:

1. **Age**:
   - Imputed missing values using the **median** of the column.

2. **Cabin**:
   - Dropped the column due to a large number of missing values, or alternatively, a feature indicating whether the cabin is known could be added.

3. **Embarked**:
   - Imputed missing values with the **most frequent value** (mode) in the column.

## Installation

To run this project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/titanic-survival-prediction.git
   cd titanic-survival-prediction

