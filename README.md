This assignment focuses on building a machine learning model using Spark MLlib to predict energy consumption (Appliances).

First, the dataset is loaded into a Spark DataFrame, and the date column is removed since it is not needed for prediction. The first few rows are displayed to understand the structure of the data.

Next, basic exploratory data analysis (EDA) is performed using summary statistics and correlation. This helps to understand the distribution of the data and identify which features are related to the target variable.

Then, the dataset is split into training and testing sets using a 75/25 ratio with a fixed random seed to ensure reproducibility.

After that, a machine learning pipeline is created. A VectorAssembler is used to combine all input features into a single feature vector, which is required by Spark ML models. Then, a LinearRegression model is used to predict the Appliances energy consumption. The pipeline is trained using the training dataset.

Finally, the model is evaluated on the test dataset. R-squared and RMSE are calculated to measure the model performance. R-squared shows how well the model explains the data, and RMSE shows the average prediction error. The most important features are also identified based on the model coefficients, which helps to understand which variables have the biggest impact on the prediction.

Overall, this assignment demonstrates the end-to-end process of data preprocessing, model building, and evaluation using Spark MLlib.
