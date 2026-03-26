# Insurance-Purchase-Prediction-Model

Overview
This notebook demonstrates a basic binary classification task using Logistic Regression to predict whether an individual will purchase insurance based on their age. The process covers data loading, exploratory data analysis, data splitting, model training, evaluation, and manual prediction using the model's coefficients.

Dataset
The dataset insurance_data.csv contains two columns:

age: The age of the individual.
bought_insurance: A binary variable indicating whether the individual bought insurance (1 for Yes, 0 for No).
Steps Performed
Data Loading and Initial Exploration: The dataset is loaded into a pandas DataFrame, and its head is displayed.
Visualization: A scatter plot is generated to visualize the relationship between age and the likelihood of buying insurance.
Data Splitting: The dataset is split into training and testing sets (80% for training, 20% for testing) using train_test_split from sklearn.model_selection.
Model Training: A LogisticRegression model from sklearn.linear_model is initialized and trained on the training data (X_train, y_train).
Model Evaluation: The trained model's performance is evaluated by:
Making predictions on the test set (X_test).
Calculating prediction probabilities using model.predict_proba(X_test).
Calculating the model's accuracy score using model.score(X_test, y_test).
Model Interpretation: The model.coef_ (coefficient) and model.intercept_ (intercept) are extracted to understand the learned relationship.
Manual Prediction Function: A custom sigmoid function and prediction_function are defined to manually replicate the logistic regression prediction based on the learned coefficient and intercept.
Key Concepts Demonstrated
Logistic Regression for binary classification.
Data splitting for training and testing.
Model training and evaluation metrics (accuracy, prediction probabilities).
Understanding of coefficients and intercepts in logistic regression.
Implementation of the sigmoid activation function.
