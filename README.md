# AdaBoost_Regressor_using_Abalone_Dataset
In this notebook, we will train an AdaBoost Regressor for a small regression problem.

We are using the Abalone dataset http://archive.ics.uci.edu/ml/datasets/Abalone
which is a small dataset suitable for regressing (predicting) the numbers of rings of new abalone instances. The dataset contains 8 attributes. The ring values are what we want our AdaBoost regressor to predict.
The data and description about the attributes can be downloaded, respectively, from
http://archive.ics.uci.edu/ml/machine-learning-databases/abalone/abalone.data
http://archive.ics.uci.edu/ml/machine-learning-databases/abalone/abalone.names
For this notebook, we the datafile is abalone.data

The tasks done in this notebook are as follows.
1. Inspecting the data and performing the following data cleaning steps:
i) from the correlations between pairs of features, determining which two features should be removed for the subsequent training and testing steps, with explanation on why them.
ii) for the text column, relabeling the ’M’ and ’F’ instances in our code as ’A’ (abbrev. for Adult). Using one-hot encoding1 to convert this column into numerical columns.
2. Performing a random 85/15 split of the data to form a training set and a test set.
3. For the AdaBoost Regressor, using the Support Vector regressor SVR with an RBF kernel as the base estimator. 
4. As the ring values must be integers, we should round and cast the predicted outputs from the ensemble regressor into integers. 
5. Reporting the mean absolute errors (MAEs) (both numerically and graphically) of all the intermediate and the final models.
6. Plotting the prediction results.
7. Plotting the distributions of the raw prediction errors of the final model.
8. Comparing the performance of the AdaBoost regressor on the training and test sets and providing a brief summary.
