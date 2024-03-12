# Regression

Project Name - Seoul Bike Sharing Demand Prediction
Project Type - Regression
Contribution - Individual
Team Member 1 - Kiran
Technical part:

Dataset file has 8760 rows and 14 columns.

Features of the dataset are as below: 'Date', 'Rented Bike Count', 'Hour', 'Temperature(°C)', 'Humidity(%)', 'Wind speed (m/s)', 'Visibility (10m)', 'Dew point temperature(°C)', 'Solar Radiation (MJ/m2)', 'Rainfall(mm)', 'Snowfall (cm)', 'Seasons', 'Holiday', 'Functioning Day'.

Target variable is: 'Rented Bike Count'

Data tyes of variables: All variables are in numeric form except four variables viz. data, seadon, season and functioning day which were in object form.

Null Values: No null values were there.

Duplicate Values: No duplicate values were there.

Important features: Features 'temperature','Dew point temperature ' 'Solar Radiation ' 'Visibility ' and 'Wind speed', were of prime importance.

Project Summary -
During our analysis, we began by performing Exploratory Data Analysis (EDA) on all the features in our dataset. We started with the dependent variable, 'Rented Bike Count,' and applied necessary transformations. Afterwards, we proceeded to analyze the categorical variables, dropping those with a dominant single class. Additionally, we examined the numerical variables, investigating their correlation, distribution, and relationship with the dependent variable. Certain numerical features with predominantly 0 values were removed, and we applied one-hot encoding to the categorical variables.

Based on correlation matrix we can say that for 'Rented Bike Count' there is a positive correlation with 'temperature(0.53)', 'Wind speed(0.12)', 'Visibility (0.19)', 'Dew point temperature (0.37)' and 'Solar Radiation (0.26)'. Also we have found some negative correlations for 'rented bike count' with 'humidity', 'rainfall' and 'snowfall'

Moving forward, we implemented five machine learning algorithms, namely Linear Regression, Lasso and Ridge, random forest, gradient boosting. To enhance our model's performance, we performed hyperparameter tuning with ridge model but it yielded with no positive site. Beacause after hyperparameter tuning, the changes in the evaluation metrics were negligible.

Based on the outputs of the evalution matrics of implemented models, it seems that both ***Random Forest Regression and Gradient Boosting Regression are strong performers** for our dataset, with Random Forest Regression slightly edging out Gradient Boosting Regression in terms of R-squared and RMSE.

Random Forest Regression outperforms Gradient Boosting Regression on both the training and testing datasets. It achieves lower error metrics on the testing data, with an MAE of 2.240 and an RMSE of 3.534, compared to Gradient Boosting Regression's MAE of 3.499 and RMSE of 4.610. Additionally, Random Forest Regression has a higher R-squared value on the testing data, with 0.919 compared to Gradient Boosting Regression's 0.862. These results indicate that Random Forest Regression demonstrates better overall performance and generalization to unseen data. Therefore, for this task, Random Forest Regression is the recommended choice.

Therefore, if you are looking for the best model between the two for your task ** Random Forest Regression seems to be the better choice** based on the outcomes of the evaluation metrics.

Nevertheless, this is not the final conclusion. Given the time-dependent nature of the data, variables such as temperature, windspeed, and solar radiation may exhibit inconsistencies over time. Consequently, there will be instances where the model's performance may suffer. As Machine Learning is continuously advancing, it is essential to remain vigilant and prepared for any unforeseen circumstances. Regularly monitoring and updating our model will be crucial to its success. Thus, possessing a solid foundation of knowledge and staying abreast of the ever-evolving ML landscape will undoubtedly provide an advantage for the future.
