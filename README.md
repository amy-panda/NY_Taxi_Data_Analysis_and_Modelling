# New York Taxi Trips - Data Analysis and Predictive Modelling
This project focuses on the taxi trips in New York City from 2019 to 2022 and performs data processing, transformation as well as analysis with Databricks Spark to provide business findings and insights. Two algorithms - Multiple Linear Regression and Decision Tree are used to build regression models, aimed at predicting the total fare amount of taxi trips based on the features like trip duration, taxi speed, tips and so on. 

## Data Ingestion
The flow chart below illustrates the process for data ingestion and preparation using both Azure and Databricks. 
![DataIngestion](https://github.com/amy-panda/NY_Taxi_Data_Analysis_and_Modelling/blob/main/images/Data%20Ingestion.jpg)

## 📊 Key Insights
- During the week, Thursday and Friday were commonly seen to have the most trips. During the day, 3pm and 6pm were the busiest time for taxi drivers. 
- Taxi drivers received a tip in majority of the trips, around 70%. In 2.6% of these trips, the driver received a tip of at least $10. 
- Compared to yellow taxi, green taxi trips had a higher average and median value for trip duration, distance and speed. In contrast, the maximum values for trip duration, distance and speed are all higher during yellow taxi trips. 




## 🏗 Predictive Models
The features used to predict the total fare amount of taxi trips include trip distance, trip duration, toll amount, tip amount, airport fee and car speed. The dataset is split into training and testing sets with the 80-20 ratio, followed by the data processing with VectorAssembler and ML Pipelines. Two algorithms - Multiple Linear Regression and Decision Tree are leveraged to build predictive models. The Root Mean Square Error (RMSE) score for each model is presented in the table below. 


|ML Model                         | RMSE - training set |RMSE - test set 
|---------------------------------|---------------------|-----------------         
|Multiple Linear Regression (MLR) |3.0517               |3.0577
|Decision Tree (DT)               |3.8250               |3.8257

Compared to the DT model, the MLR model gives a lower value of RMSE for both training and test sets. Thusthe MLR model is regarded as a better model to predict the total fare of taxi trips. &nbsp; 

## 🛠 Techniques and Tools Used
- Databricks
- Azure
- Spark SQL
- MLlib
- Pyspark
- Multiple Linear Regression
- Decision Tree

## ℹ️ Data Source