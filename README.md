House Price Prediction - Machine Learning Project
Overview:
This project focuses on building a supervised machine learning model to predict house prices in California. We used various techniques like feature engineering, model training, and evaluation to improve the prediction accuracy. The project was structured as follows:

Project Structure:
1. Data Loading and Preparation
Loaded the train and test datasets using pandas.
Verified the data by displaying the first five rows.
Split data into train and test sets without re-splitting the original datasets.


2. Exploratory Data Analysis (EDA)
Statistical Summary: Displayed descriptive statistics using train_data.describe().
Visualizations:
Scatter plot between median income and house prices.
Histogram to show the distribution of house ages.
Heatmap to display correlations between the features.
Boxplots to analyze house prices by age and location clusters.


3. Feature Engineering
Created new features:
MedInc^2: Square of the median income to capture non-linear relationships.
log_MedInc: Logarithmic transformation of median income for normalization.
Ratios such as RoomsPerHouse and BedroomsPerRoom.
Applied KMeans clustering to group houses by geographic location (Latitude and Longitude).


4. Model Training and Hyperparameter Tuning
Used Random Forest Regressor for predicting house prices.
Optimized model parameters (n_estimators and max_depth) using Grid Search with 5-fold cross-validation.
Selected the best parameters based on the lowest Mean Squared Error (MSE).


5. Model Evaluation and Prediction
Predicted house prices on the test dataset.
Measured model accuracy using Root Mean Squared Error (RMSE).
Printed the first five predictions to showcase the model's performance.


Key Libraries:
pandas, numpy: Data manipulation and numerical computations.
seaborn, matplotlib: Data visualization.
sklearn: Machine learning algorithms, model evaluation, and feature scaling.
Results:
The optimized Random Forest model achieved a low RMSE, indicating accurate predictions for house prices based on the input features.
The visualizations and correlations helped identify key factors like median income and geographical location that heavily influence house prices.
