# Flight Price Prediction
# Introduction
As a not financially comfortable college student, I want to build a model to predict the flight fares given (1) location, (2) time, and (3) destination. The core reason for this project is, besides being a solid Bachelor's level ML project, to predict the cheapest time that I can buy flight tickets to go back to Vietnam and see my parents. But that feature is still under development as I need to find a way to scrape real time data from Skyscanner. For now, I'm using a dataset that I found on Kaggle.

# Goal
- Objective: Develop a ML model to predict flight fares.
- Benchmarking: The approach is benchmarked against existing solutions from top flight booking platforms (Google Flights, Skyscanner).

## Dataset

The [Dataset](https://www.kaggle.com/datasets/nikhilmittal/flight-fare-prediction-mh/code?datasetId=140442&sortBy=dateCreated) used in this project contains information about flight details and prices. 

Key features include:

- Airline: The airline operating the flight
- Source: The starting point of the flight
- Destination: The endpoint of the flight
- Duration: Total duration of the flight
- Total_Stops: Number of stops between the source and destination
- Additional_Info: Additional information about the flight
- Price: Price of the flight ticket
  
## Libraries Used

- pandas
- matplotlib
- seaborn
- numpy
- scikit-learn
- xgboost
- 
## Models Used

- Linear Regression
- ElasticNet
- Ridge Regression
- Lasso Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- AdaBoost Regressor
- Support Vector Regressor (SVR)
- XGBoost Regressor
- 
# Results
The models are evaluated based on their performance metrics: RMSE (Root Mean Squared Error) and R-squared score. The XGBoost Regressor is found to be the best-performing model for this dataset.

| Model                         | RMSE     | R2 Score  | Score    |
|-------------------------------|----------|-----------|----------|
| Lasso                         | 0.364501 | -0.965990 | 0.404442 |
| ElasticNet                    | 0.361464 | -0.510280 | 0.414326 |
| RidgeCV                       | 0.305209 |  0.271923 | 0.582439 |
| LinearRegression              | 0.305209 |  0.271934 | 0.582439 |
| SVR                           | 0.294032 |  0.488338 | 0.612462 |
| AdaBoostRegressor             | 0.255574 |  0.274876 | 0.707208 |
| GradientBoostingRegressor     | 0.164851 |  0.851156 | 0.878182 |
| DecisionTreeRegressor         | 0.146908 |  0.903038 | 0.903258 |
| RandomForestRegressor         | 0.113365 |  0.939124 | 0.942392 |
| XGBRegressor                  | 0.106426 |  0.946901 | 0.949228 |


