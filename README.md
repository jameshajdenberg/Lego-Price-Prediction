# Lego-Price-Prediction

In this project, I utilized skills learned in my Foundations of Data Science class to perform Exploratory Data Analysis, test models, and predict future price points for arbitrary lego sets. Below is a quick summary of what actions were performed in the project above. For further detail and for visualizations, download both the ipynb and included csv. 

Initial Data Assessment:

Removed irrelevant columns such as Number, multi-currency Price columns, and time-related columns (Launch date, Exit date).
Dropped Weight, Height, and Depth columns as non-critical factors in price prediction.
Imputed missing values (e.g., Minifigs NaN values converted to 0).
Addressed null values in the subtheme column, but kept it temporarily for validation purposes.
Data Cleaning Process:

Removed "Promotional" LEGO sets as they do not contribute to general price prediction due to their event-specific nature.
Excluded unreleased sets (e.g., those coming out in 2024) due to incomplete price data.
Feature Engineering:

Added columns to classify LEGO sets by their overarching genre (e.g., action, educational).
Created a column identifying whether a set is based on an intellectual property (e.g., TV shows, movies) or is an original LEGO set.
Introduced a column mapping each year to the corresponding inflation rate to adjust price analysis for inflation.
Exploratory Data Analysis (EDA):

Identified categorical features (e.g., Theme, Genre, Set Name) and numerical features (e.g., Year, Pieces, RRP).
Finalized the dataset by removing null values and confirming data types.
Model Testing:

Tested and compared multiple models (Linear Regression, SVR, and Random Forest Regression) to predict LEGO set prices.
Linear Regression and SVR models initially tested, but Random Forest Regression (RFR) provided the best R-squared value (0.84), making it the chosen model for price prediction.
