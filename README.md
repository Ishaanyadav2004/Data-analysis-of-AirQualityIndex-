# Data-analysis-of-AirQualityIndex-

 # Introduction
 We aim to predict the AQI for different states across India and perform data analysis and also apply various machine learning techniques. By leveraging data on key pollutants(Sulphur Dioxide (SO2), Nitrogen Dioxide (NO2), Particulate Matter (PM10 and PM2.5) , Carbon Monoxide (CO), Ozone(O3) etc.) recorded in real time we seek to develop predictive models capable of estimating AQI values for all the states in India. 
We used machine learning models, such as linear regression, support vector machines (SVM), random forest, gradient boosting machines (GBM), and decision trees, to predict the average pollutant values.
We also evaluated performance of each model using appropriate evaluation metrics, including mean absolute error (MAE), mean squared error (MSE), root mean squared error (RMSE), and R-squared and then comparing them.
# Dataset Description
The dataset is taken from data.gov.in website. It has state-wise data for different pollutants recorded across various cities with their respective geographic coordinates. 

# Algorithm Used
Data Cleaning – The NA values in pollutant_min, pollutant_max, pollutant_avg columns are replaced by mean of the values in the column group-wise for each pollutant.
Descriptive statistics – The mean, median, mode, standard deviation, and variance are calculated for pollutant_avg for each pollutant.
AQI calculation – The AQI values are calculated on the basis of Indian standards for each category of pollutant for each state. The overall AQI for a particular state is taken to be the maximum AQI value of any pollutant. Also, the AQI values are then categorized to be "Good", "Satisfactory", "Moderate", "Poor", "Very Poor", "Severe“ as per the standards.
# Machine learning models 
LINEAR REGRESSION : Linear regression is a simple yet powerful statistical technique which assumes a linear relationship between the predictor variables and the response variable.
RANDOM FOREST : Random Forest builds multiple decision trees during training and combines their predictions through averaging or voting to improve accuracy and reduce overfitting. It is particularly effective for both classification and regression tasks, handling large datasets with high dimensionality and complex interactions.
SUPPORT VECTOR MACHINE (SVM) : Support Vector Machine is used for classification and regression tasks. It works by finding the optimal hyperplane that separates data points into different classes while maximizing the margin between classes. SVMs are effective in high-dimensional spaces and are capable of handling non-linear relationships through the use of kernel functions.
GRADIENT BOOSTING MACHINE (GBM) : Gradient Boosting Machine builds a strong predictive model by sequentially adding weak learners (typically decision trees) to minimize the loss function. GBM iteratively improves the model by focusing on the errors made by the previous models, resulting in higher predictive accuracy.
DECISION TREE : Decision Tree partitions the feature space into smaller regions based on feature values, making decisions at each node to predict the target variable. Decision trees are intuitive, easy to understand, and capable of capturing non-linear relationships in the data.

