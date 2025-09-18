# What-Drives-the-Price-of-a-Car-
Required Assignment 11.1: What Drives the Price of a Car?

Project Overview
This project applies the CRISP-DM (CRoss-Industry Standard Process for Data Mining) framework to analyze a large-scale dataset of over 426,000 used cars. The core objective is to move beyond simple data exploration and build a robust predictive model that uncovers the most significant drivers of a used car's price. The ultimate goal is to provide a used car dealership with actionable, data-driven insights to optimize their inventory acquisition and pricing strategies, giving them a competitive advantage in the market.

The CRISP-DM Process
The project is structured according to the six phases of the CRISP-DM methodology:
Business Understanding: We defined the business problem as identifying factors influencing car prices to help a dealership make smarter inventory and pricing decisions. This was translated into a technical goal: building a regression model to predict price.
Data Understanding: Initial exploration of the raw data revealed a variety of features, including numerical and categorical types, and highlighted critical issues like missing values and outliers in key variables like price and odometer.
Data Preparation: This phase involved extensive data cleaning, including dropping irrelevant columns, handling outliers, and imputing missing values. A new, more insightful car_age feature was engineered, and categorical features were optimized and prepared for modeling through one-hot encoding.
Modeling: We built a Random Forest Regressor model, which is well-suited for this type of problem. To ensure the model was robust and efficient, we used RandomizedSearchCV with cross-validation on a subset of the data to find the optimal model hyperparameters.
Evaluation: We evaluated our model's performance using Mean Absolute Error (MAE) and R-squared (R2) metrics. Crucially, we analyzed the model's feature importance to identify the true drivers of price, providing the direct answer to our business question.
Deployment: The final output is a clear, non-technical report summarizing our findings and providing direct, actionable recommendations for the dealership's business operations.

Key Findings
Our analysis, backed by a high-performing model, reveals the following key drivers of used car prices:
Mileage is the #1 Factor: A car's odometer reading is the most significant predictor of its price. The relationship is strongly inverse; lower mileage leads to a higher price.
Age is a Close Second: The age of a vehicle is the second most important factor, as it's a direct indicator of depreciation.
Make and Model Matter: Certain manufacturers and models, such as Toyota and Honda, consistently hold their value better than others.
Condition and Features Add Value: We found that factors like a clean title, "excellent" condition, and an automatic transmission can add a noticeable premium to a car's price.

Notebook & Code
The full analysis, including all code and visualizations, is detailed in the accompanying Jupyter Notebook:  https://github.com/nbuddi/What-Drives-the-Price-of-a-Car-/blob/main/prompt_II.ipynb
