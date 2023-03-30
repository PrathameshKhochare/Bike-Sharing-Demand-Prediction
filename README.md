# Bike-Sharing-Demand-Prediction
This project aims to enhance the mobility and convenience of the public through bike-sharing programs in metropolitan areas. One of the main challenges is maintaining a consistent supply of bikes for rental.
![image](https://user-images.githubusercontent.com/121234763/228830841-29d03322-0a3c-4c2b-9c98-19c2bf63c078.png)
# Problem statement:
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.
# Dataset
The dataset is from Seoul's Bike Sharing Program. The data set includes over 8000 records and 14 attributes based on historical usage patterns, including temperature, time, and other data.For more information on the dataset, please visit the Kaggle website at 
"https://www.kaggle.com/datasets/saurabhshahane/seoul-bike-sharing-demand-prediction"
# Dataset description:
The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.

Attribute Information:

* Date : year-month-day
* Rented Bike count - Count of bikes rented at each hour
* Hour - Hour of he day
* Temperature-Temperature in Celsius
* Humidity - %
* Windspeed - m/s
* Visibility - 10m
* Dew point temperature - Celsius
* Solar radiation - MJ/m2
* Rainfall - mm
* Snowfall - cm
* Seasons - Winter, Spring, Summer, Autumn
* Holiday - Holiday/No holiday
* Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)

## Project Flowchart:
Initial preparations(Loading the dependencies and the data)

EDA
1. Know Your Data
2. Understanding your Data
3. Data Wrangling
  * Handling null values
  * Handling duplicate values
  * Removing Outliers
  * Feature engineering

4. Data Vizualization, Storytelling & Experimenting with charts : Understand the relationships between variables
5. Hypothesis Testing
6. Feature encoding
    * Outlier treatment
    * Linearity check
    * Removing Multicollinearity
    * Categorical Encoding
    * Data Transformation
7. Model Building
    * Train Test Split
    * Scaling Data
    * Model Training
    * Model Implementation
8. Model Result 
    * Linear models-
     * Linear Regression
     * Ridge Regression
     * Lasso Regression
     * ElasticNet
   * Tree based models-
     * Decision Tree
     * Random forest regression
     * AdaBoost
     * XGBoost
     * LGBoost
   * Other
     * KNN
     * SVM
9. Model explainability
10. Conclusion

![image](https://user-images.githubusercontent.com/121234763/228838111-825a316d-39e7-4a6a-96ec-2ca3c7a01005.png)
## Conclusion
1. EDA insights:

Most number of bikes are rented in the Summer season and the lowest in the winter season.
Over 96% of the bikes are rented on days that are considered as No Holiday.
Most number of bikes are rented in the temperature range of 15 degrees to 30 degrees.
Most number of bikes are rented when there is no snowfall or rainfall.
Majority of the bikes are rented for a humidity percentage range of 30 to 70.
The highest number of bike rentals have been done in the 18th hour, i.e 6pm, and lowest in the 4th hour, i.e 4am.
Most of the bike rentals have been made when there is high visibility.

**Cateforical Features-**
* Season - As we can see that summer has the highest number of bikes rented, 37%. This could be because of the vacation mood created in summer and also the increase in the number of tourists. Winter however is the season where the least number of bikes are rented, 8%.
* Holiday - In the Holiday column, The demand is low during holidays, but in no holidays the demand is high, it may be because people use bikes to go to their work.
* Fuctioning Day - If there is non Functioning Day then there is no demand
* Week - Bike demand is High during Afternoon during Weekends.
         While there is more demand during office hours in weekdays (7am to 9am  and 5pm to 8pm)
* Month -Demand is low in November, December January & February, It is cold in these months and we have already seen in season column that demand is less in winters.**
*Year -The demand was less in 2017 and higher in 2018.

**Numerical Features-**
* Temperature - As we can see that the most number of bikes rented are in the temperature range of 15 degrees to 30 degrees.
* Humidity - As we can see that the majority of the bikes are rented for a humidity percentage range of 30 to 70.
* Wind Speed - As we can see that higher bike rented count is for Wind speed between 0 to 5 m/s
* Visibility - We can see that higher visibility is preffered by the customers.
* Dew Point Temperature -The average number of bikes rented with dew point temperature increases steadily.
* Rainfall - People prefer almost no or very less rainfall.
* Snowfall - People prefer almost no or very less snowfall.

**ML Model Insights:**
* I have chosen the Light GBM model because it has the lowest RMSE value as well as the highest R2 score on the test data.
* Due to less no. of data in the dataset, the training R2 score is around 98% and the test R2 score is 99%. Once we get more data we can retrain our algorithm for better performance.
* I have used Eli5 for Model Explainability.

**For further information you can check the google colab file added in the repository.

**If you find any mistakes or have any suggestions for me, please reach out to me, all the criticism is heartly welcomed.

**You can also reach out to me for project collaborations.

**My Email Id - khochareprathamesh10@gmail.com

