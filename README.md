# Data Analytics & Machine Learning _Practical Test
The practical test is to assess on analytical thinking, initiate appropriate steps for data processing and develop and validate machine learning algorithms.
## What is the test about?
The data used in the test involves data from multiple chains of medical outlet. The dataset comes in two files, namely "train" and "test" set. The missing values are identified to be Missing Not At Random (MNAR). A classification algorithm is to be developed to classify the outlet type
based on the "OutletSalesPerHour" column (label). 
These are the highlight of the practical test:
* Feature engineering is performed by combining both the train and test file and a new unique ID identifier is created from the combination of "OutletIdentifier" and "OutletLocation".
* K-Nearest Neighbour model is used to impute the missing values in "OutletSize" column.
* Random Forest Regression model is used to impute the missing values in "B40PatientPerDay" column.
* Values in label column is categorize using the first and third quartile.
* Oversampling is used to balance the data by increasing the minority class for the model to learn.
* A random forest classifier is then defined with a random seed of 42, a n_estimators of 80 as it is the best parameter after trial and errors and the class_weight is balanced to ensure that the model calculate and assign appropriate weights based on the class distribution since the data for the target column is quite imbalance.
* 
