# What I have Done in the Project.
       * Importing the Libraries
       * Read the Data
       * Getting information about data like how many null values in the data, how many features in the data, etc
       * Exploratory Data Analysis on the dataset: Regression Plot, Boxplot, Barplot,etc
       * Skewness and outlier Handling
       * Checking Multicollinearity of data using Correlation matrix and VIF and dropping those columns who has high correlation and VIF
       * One hot encoding on categorical data
       * Splitting the data for Training and Testing the model
       * Standardising the Independent variable
       * Performing different model
       * Using LIME, getting the insights about the data that which features is impacting the data positively and negatively
  
 # Different Models which are used in the Project:
       * Linear Regression
       * Ridge Regression
       * Decision Tree Regressor with GridSearchCV
       * Random Forest
       * Gradient Boosting Regressor
       * Gradient Boosting with GridSearchCV
       * XGBoost with RandomisedSearchCV
       
 # Conclusion:
             * Count of Rented Bike(dependent variable) : positively skewed
      * Normally distributed attributes:
                    - Temperature
                    - Humidity
      * Positively skewed attributes:
                    - Wind 
                    - Solar Radiation 
                    - Snowfall 
                    - Rainfall
      * Negatively skewed attributes: 
                    - visibility
      * Positively correlated variables to the bike rent are :
                    - Temperature
                    - Dew Point Temperature
                    - Solar Radiation
                    - Hour

      * And most negatively correlated variables are:
                    - Humidity
                    - Rainfall
                    - Weekdays or Weekends
      * The number of bikes rented is on average higher during the rush hours.i.e. at 6 p.m. to 8 p.m.
      * The rented bike counts is higher during the summer and lowest during the winter.
      * The rented bike count is higher on working days than on non-working days.
      * On a non-functioning day, no bikes are rented in all the instances of the data.
      * The number of bikes rented on average remains constant throughout Monday - Saturday, it dips on Sunday, and on average, the rented bike counts is lower on weekends than on weekdays.
      * On regular days, the demand for the bikes is higher during rush hours. On holidays or weekends, the demand is comparatively lower in the mornings, and is higher in the afternoons.

      * Conclusion after using different models:

            - No overfitting is seen.
            - Random forest Regressor, Gradient Boosting gridsearchcv, XbBoost Regressor with GridSearchCV gives the highest R2 score .
            - Feature Importance value for Random Forest, Gradient Boosting, XgBoost are different.
            - We can deploy Random Forest, Gradient Boosting with  GridSearchCV, XgBoost with RandomizedSearchCV model.

      * Important Feature which affect the most in the rented bike count:

          * Functioning Day
          * Winter Season
          * 18th Hour i.e. 6 p.m.
          * Temperature
          * Humidity

      * Features wich impact Negatively on Rented Bike Count:  

          * Hour 4 i.e. 4 a.m.
          * Hour 5 i.e. 5 a.m.
          * Hour 3 i.e. 3 a.m.
          * Winter Season 
          * Rainfall 
          * weekdays_weekend

      * Features wich impact Positively on Rented Bike Count:

          * Hour 18 i.e. 6 p.m.
          * Hour 19 i.e. 7 p.m.
          * Hour 8 i.e. 8 a.m.
          * Hour 21 i.e. 9 p.m.
          * Hour 20  i.e. 8 p.m.
