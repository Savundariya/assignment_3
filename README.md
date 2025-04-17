# assignment_3
PowerPulse: Household Energy Usage Forecast
# Files
Machine_learning_models.ipynb
Trains and evaluates models with outliers in the dataset.

# Machine_learning_models_without_outliers.ipynb
Trains and evaluates models after removing outliers, potentially improving performance.

#Dataset
Source: UCI Machine Learning Repository
Contains measurements of electric power consumption in one household over four years.
Key features include: Global_active_power, Global_reactive_power, Voltage, Global_intensity, Sub_metering_1/2/3.

# Project Workflow
1. Data Loading & Exploration
Data fetched via ucimlrepo.
Initial structure examined using .info() and .describe().
2. Data Preprocessing
Datetime parsing and feature extraction (hour, day, weekday, etc.).
Handling of missing and non-numeric entries.
Normalization via StandardScaler.
In the without outliers notebook:
Outliers are removed using IQR method on Global_active_power.
3. Feature Engineering
Additional time-based features.
4. Model Training
Models Used:
Linear Regression
Random Forest Regressor
Gradient Boosting Regressor
Neural Network (MLPRegressor)

# Steps:
Train-test split (80/20).
Model fitting and prediction.
Evaluation using:
RMSE (Root Mean Squared Error)
MAE (Mean Absolute Error)
R² Score
5. (Optional) Hyperparameter Tuning
Hyperparameter tuning using GridSearchCV have been added for Randomforest Model 

# Results
You can compare performance with and without outliers using evaluation metrics. Removing outliers often improves:
Model accuracy
Generalization to unseen data

# How to Run
Clone the repository or download the .ipynb files.
# Install dependencies:
pip install ucimlrepo scikit-learn pandas numpy matplotlib seaborn
Run notebooks in Jupyter or VS Code.
