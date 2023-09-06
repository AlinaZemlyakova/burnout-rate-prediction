# Burnout Rate Prediction
This project is aimed at studying the predisposition to burnout in the workplace. The dataset was selected as the research material can be found via link (also added here as zip file): https://www.kaggle.com/datasets/blurredmachine/are-your-employees-burning-out

**Dataset contains the following data:**
* Employee ID: The unique ID allocated for each employee (example: fffe390032003000)
* Date of Joining: The date-time when the employee has joined the organization (example: 2008-12-30)
* Gender: The gender of the employee (Male/Female)
* Company Type: The type of company where the employee is working (Service/Product)
* WFH Setup Available: Is the work from home facility available for the employee (Yes/No)
* Designation: The designation of the employee of work in the organization.
        In the range of [0.0, 5.0] bigger is higher designation.
* Resource Allocation: The amount of resource allocated to the employee to work, ie. number of working hours.
        In the range of [1.0, 10.0] (higher means more resource) 
* Mental Fatigue Score: The level of fatigue mentally the employee is facing.
        In the range of [0.0, 10.0] where 0.0 means no fatigue and 10.0 means completely fatigue.
* Burn Rate: The value we need to predict for each employee telling the rate of Burnout while working.
        In the range of [0.0, 1.0] where the higher the value is more is the burn out.

**The project consists of the following steps:**
1) data visualisation and EDA
2) creating a baseline linear regression model
3) evaluating the effectiveness of regression via MSE, RMSE, MAE
4) feature engineering
5) model testing (KNeighborsRegressor, DecisionTreeRegressor with GridSearchCV, XGBoost with tuning)
6) cross-validation, models performance comparison
