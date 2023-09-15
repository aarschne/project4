# Machine Learning Analysis of You Tube Metrics
The project is about predicting the views and revenue of you tube videos using Machine Learning models. The models used in the project are Deep Learning Regression, K-Means Clustering and Agglomerative Clustering.

# Objectives
* To use unsupervised learning model “K-Means” to predict clusters of YouTube videos.
* To use supervised learning model “Keras” to predict the revenue generated by YouTube videos.
* To use supervised learning model “Keras” to predict the number of views of YouTube videos
* To tune the supervised learning model to find the best hyperparameters.

# Getting Started
1. ETL - First of all the data was extracted from Kaggle using this link  https://www.kaggle.com/datasets/thedevastator/youtube-analytics-how-to-keep-your-viewers-engag. The data has 3 csv files and we decided to use two of them. The data was cleaned by dropping some columns and renaming the columns. The null values in the data were found and some rows were deleted.
2. Standard Scaler from scikit  is used to standardize the data and heat map is drawn using Seaborn to show the correaltion between the features.![image](https://github.com/aarschne/project4/assets/128007832/25b1502e-3444-4cb1-8da1-bdf67073e0e7)

3. Clustering is done using K- Means Clustering and Agglomerative Clustering.
4. In the next step, the Deep Learning Regression model is developed for the same data.
5. The cost per 1000 views column is multiplied by number of views and then divided by 1000. For the label the same thing is done but with Revenue per 1000 views.![image](https://github.com/aarschne/project4/assets/128007832/af375df8-56f6-4330-8540-39d76d73e0ef
 
6. The data is  preprocessed into a training and testing dataset.
7. The data is standardized and Keras Regressor model is defined with six hidden layers and an output layer with one unit.
8. The model is compiled and trained and mean absolute percent error of 424.52 is achieved on the test data.
9. Keras tuner is used to find better parameters.
10. Best model had mean absolute percentage error of 37.8564 during validation.

# Results
1. In the first attempt test data had mean squared error of 7036.71 and Root mean error was 83.89. The mean of the revenue column is 132.21, and the max is 7963.86.
2. We had some overfitting in the first attempt.![image](https://github.com/aarschne/project4/assets/128007832/bb32593e-70ff-4b6f-b5de-831e3bb4b8bb)
3. We decided that absolute percent error was a better loss function.
4. After using Keras tuner best model has mean absolute percentage error of 37.8564 during validation.

# Contributors
 * Aaron Schneberger https://github.com/aarschne
 * Ashok Goyal 
 * Navyasri Pusuluri
 * Roli Singh https://github.com/rolisingh10

 # Acknowledgements
   We would like to thank our instructor Shaun Mcpeck and teaching assistant William Vann for their help and guidance.
 



   
 
    
