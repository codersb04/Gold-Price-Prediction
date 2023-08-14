# Gold-Price-Prediction
## Task:
Build a Machine Learning model to predict the prices of gold.</br>
This comes under Supervised learning as we have provided labelled data. As in this problem, we need to predict the prices in this so we used a regression model that is Random Forest Regression to achieve the task. Random Forest Regression uses multiple decision trees to get the result.
## Dataset:
The dataset contains information about the prices of gold in a range of years from 2008 to 2018. The dataset contains 2290 records of different years with 6 features. The features are:</br>
. Date: Non-Null, Date Type </br>
. SPX: Non-Null, Float Type   </br>
. GLD: Non-Null, Float Type</br>
. USO: Non-Null, Float Type</br>
. SLV: Non-Null, Float Type</br>
. EUR/USD: Non-Null, Float Type</br></br>

Source: https://www.kaggle.com/datasets/altruistdelhite04/gold-price-data

## Steps Involved:
### Import Dependencies
The libraries needed to achieve the result are:</br>
. pandas</br>
. numpy</br>
. matplotlib.pyplot</br>
. seaborn</br>
. RandomForestRegressor from sklearn.ensemble</br>
. train_test_split from sklearn.model_selection</br>
. metrics from sklearn</br>

### Data Collection and Processing
. Use read_csv function from pandas to import the dataset. </br>
. Use the function such as shape, describe, head, and info to know more about the data set.</br>
. Check for the missing value using the isnull function.</br>
. Split the dataset into features and labels(Target). The label will contain the column GLD(Gold Price) and the feature will contain the rest of the column except Date(as it is hard for the machine to process) and GLD(Gold Price).
### Data visualization
. Construct a heatmap to know about the positive and negative correlation between all the features.</br>
. Plotted a distribution graph which shows how the gold price is distributed over the whole dataset.

### Model Training and Evaluation
. Split the dataset into training and test data. We have taken 20% of the for test purposes and the rest 90% for the training.</br>
. We have used Random Forest Regressor to achieve the result. </br>
. Prediction and Evaluation are being carried out for test data.</br>
. The R Square Error score for test data is 0.9890266692833741</br>
. At the last, we have plotted a graph to compare the resulted values and the actual values.</br></br></br></br>



Reference: Project 8. Gold Price Prediction using Machine Learning with Python | Machine Learning Projects, Siddhardhan, https://www.youtube.com/watch?v=9ffkBvh8PTQ&list=PLfFghEzKVmjvuSA67LszN1dZ-Dd_pkus6&index=9
