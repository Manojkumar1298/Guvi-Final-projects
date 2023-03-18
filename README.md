Customer Conversion Prediction
Problem Statement
You are working for a new-age insurance company and employ
multiple outreach plans to sell term insurance to your
customers. Telephonic marketing campaigns still remain one of
the most effective ways to reach out to people however they
incur a lot of cost. Hence, it is important to identify the
customers that are most likely to convert beforehand so that
they can be specifically targeted via call. We are given the
historical marketing data of the insurance company and are
required to build a ML model that will predict if a client will
subscribe to the insurance.

SOLUTION:
STEPS INVOLVED IN THIS PROJECT:
1.Importing the required libraries.
2.Import the dataset.
3.It is a binary classification problem,so it is necessary to check whether target variable is balanced or not.
4.DATA CLEANING:
             1.Checking for the null values.
             2.Spelling correction in the columns.
             3.Checking the datatypes.
             4.Checking for duplicates.
             5.Checking for outliers.
5.Explanatory Data Analysis:
             1.Distribution  of features.
             2.Feature vs Target.
6.Using correlation matrix to find the correlation between features.
7.Encoding the data.
8.Target and Feature selection.
9.Target variable is imbalanced,so we are using some of the data balancing techniques
                       1.Random undersampling.
                       2.Random oversampling.
                       3.SMOTE.
                       4.SMOTENN.
Out of theses SMOTENN gives best accuracy.
10.Splitting the model into train and test.
11.Fitting the data with different classifier models.
                          1.Logistic Regression.
                          2.Random Forest Classifier.
                          3.Decision Tree classifier.
                          4.K neighbors classifier.
                          5.XG Boost classifier.
12.Checking the feature importance of different models.
13.Out of all the classifier models Random forest classifier gives the best AUROC score pf 0.915

