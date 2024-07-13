# Titanic_Survival_Prediction

This Python script demonstrates a machine learning pipeline for predicting survival on the Titanic using various classifiers such as logistic regression, SVM , decision tree and random forest.

# Dataset Loading:
The notebook begins by loading the Titanic dataset from CSV files (train.csv and test.csv).

# Data Preprocessing:

Missing Values: Missing values in the Age, Embarked, and Fare columns are filled using median values for numerical features and mode for categorical features.

Feature Engineering: Columns like Cabin, Ticket, Name, and PassengerId are dropped as they are deemed unnecessary for the prediction task.

Categorical Encoding: Categorical variables (Sex and Embarked) are encoded using one-hot encoding to convert them into numerical format suitable for machine learning models.

Splitting Data: The dataset is split into features (X) and the target variable (y), followed by further splitting into training and validation sets using train_test_split.

Feature Scaling: Data normalization is performed using StandardScaler to standardize features for better model performance.

# Model Training and Evaluation:

Several classifiers are trained on the training data, including Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, and Support Vector Machine (SVM).
Each model's performance is evaluated using accuracy metrics on the validation set (X_val and y_val).
The best-performing model is determined based on the highest accuracy score 83% which was the random forest with Grid Search for hyperparameter tuning. (The accuracy is low because the dataset is small)

# Grid Search

Define Hyperparameters: Identify the hyperparameters for the model that you want to optimize, such as learning rate, number of estimators, or regularization strength.
Specify Grid: Define a grid of possible values for each hyperparameter.
Evaluation: Train and evaluate the model for each combination of hyperparameters using cross-validation or a validation set.
Select Best Model: Choose the combination that yields the best performance metric.


# Conclusion: 

The notebook concludes by identifying the best model and its corresponding accuracy, providing insights into which classifier performs best for predicting survival on the Titanic dataset.

