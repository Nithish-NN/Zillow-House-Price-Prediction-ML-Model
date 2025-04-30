🏡 House Price Prediction using Machine Learning
This project aims to predict house prices using the Ames Housing dataset, which contains 80 features describing different aspects of residential properties (e.g., size, quality, neighborhood). The goal is to build a robust machine learning pipeline that accurately estimates SalePrice and can be useful for real-world real estate applications.
🧠 Models Used
The following models were trained and evaluated:

Linear Regression (Baseline)

Random Forest Regressor

XGBoost Regressor (with and without tuning and weighted loss function)
🧹 Preprocessing Highlights
Outlier Removal: Removed extreme values in SalePrice using IQR.

Missing Values: Imputed numeric with mean, categorical with mode.

Feature Engineering:

Age of House

Total Bathrooms

Qual_Liv_Interaction

Total SF (total square footage)

Encoding: One-hot encoding (drop_first=True).

Transformation: Log-transformation of SalePrice.

Feature Selection: Used SelectKBest with f_regression to select top 50 features.

Scaling: StandardScaler used for consistent feature scaling.

📈 Insights
Top Features: Overall Qual, Garage Cars, Qual_Liv_Interaction, Total SF

High Correlation: Engineered features added strong predictive power.

Error Analysis: Higher prediction errors for houses >$400,000. Weighted loss improved performance in this range.

