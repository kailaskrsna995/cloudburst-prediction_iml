Weather Prediction: Machine Learning Model for CloudBurst Forecasting
Project Overview
This project aims to predict the occurrence of cloud bursts (a sudden and intense rainfall event) using weather data from various sources. By applying machine learning techniques, the goal is to build models that can predict whether a cloud burst will occur the following day based on weather parameters collected from historical data.

The project leverages multiple machine learning algorithms, including Artificial Neural Networks (ANN), Random Forest, and Long Short-Term Memory (LSTM), to evaluate the effectiveness of each algorithm in terms of prediction accuracy. The models are trained on a set of features, such as temperature, rainfall, humidity, wind speed, and more, with the target variable being whether a cloud burst occurs the next day (CloudBurstTomorrow).

Dataset
The dataset used in this project contains historical weather data with the following features:

Location

Temperature (Minimum, Maximum)

Rainfall

Evaporation

Sunshine

Wind Gust Speed

Wind Speed at 9 am and 3 pm

Humidity at 9 am and 3 pm

Wind direction (sin/cos encoded values)

CloudBurst occurrence today (CloudBurst Today)

Year, Month, Day

Target: CloudBurstTomorrow (0: No, 1: Yes)

Key Features
Data Preprocessing: Data is cleaned and normalized using Min-Max scaling to ensure the models perform optimally.

Model Training: Three machine learning models are used:

ANN (Artificial Neural Network): A neural network with multiple layers and ReLU activation functions.

Random Forest: An ensemble method using decision trees to predict cloud burst occurrences.

LSTM (Long Short-Term Memory): A type of Recurrent Neural Network (RNN) designed to handle time series data.

Model Evaluation: Each model is evaluated based on metrics such as accuracy, precision, recall, and F1-score. Confusion matrices are also generated for better insight into the models' performance.


Results & Evaluation
The results demonstrate that Random Forest outperforms the other models in terms of accuracy (86.05%) and F1-score, making it the best algorithm for predicting cloud burst events in this particular dataset. However, ANN and LSTM also show promising results, with accuracy around 85-86%. The model evaluations provide important insights into model performance and highlight areas for further improvement.

Future Work
Feature Engineering: Investigate additional weather features and time-series-based data (e.g., historical cloud burst occurrences) to improve model accuracy.

Hyperparameter Tuning: Fine-tune model parameters (e.g., learning rate, batch size, number of trees) to achieve better performance.

Deployment: Develop a web or mobile application to allow real-time cloud burst predictions based on current weather conditions.

