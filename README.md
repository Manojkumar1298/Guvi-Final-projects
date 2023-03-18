1.Customer Conversion Prediction  

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






2. StackExchange question quality detection

Aim: Categorise the StackOverflow questions into various quality classes.



SOLUTION:
STEPS INVOLVED IN THIS PROJECT:

1.Importing the required libraries.


2.Import the dataset.

3.The given data is an XML file ,so we have to parse the data using the celement tree library.

4.After parsing the data we have to extract the features from the data.

                1.Text length.
                
                2.comment count.
                
                3.Answer count.
                
                4.Score.
                
                5.Quality.
                
                6.Upvotes.
                
                7.Downvotes.

5.The target variable is created from the Score and Answer count with certain conditions.

                1. Good-Quality questions: Questions for which score is greater than 5 and answer
                  count is greater than 0 should be labelled as good quality questions.
                  
                2. Low-Quality questions: Questions for which the score is between 0 to 5 and having
                  no answers should be labelled as low-quality questions.
                  
                3. Very-low quality questions: Questions which have negative scores

After creating the features we create a feature matrix with all the features.

6.It is a multi class classification problem,so it is necessary to check whether target variable is balanced or not.


7.DATA CLEANING:

             1.Checking for the null values.
             
             2.Spelling correction in the columns.
             
             3.Checking the datatypes.
             
             4.Checking for duplicates.
             
             5.Checking for outliers.
             
             
             
8.Explanatory Data Analysis:

             1.Distribution  of features.
             
             2.Feature vs Target.
             
9.Using correlation matrix to find the correlation between features.

10.Encoding the data.

11.Target and Feature selection.

12.Target variable is imbalanced,so we are using some of the data balancing techniques

                       1.Random undersampling.
                       
                       2.Random oversampling.
                       
                       3.SMOTE.
                       
                       4.SMOTENN.
                       
Out of theses SMOTE gives best accuracy.

13.Splitting the model into train and test.

14.Fitting the data with different classifier models.

                          1.Logistic Regression.
                          
                          2.Random Forest Classifier.
                          
                          3.Decision Tree classifier.
                          
                          4.Gradient bossting classifier.
                          
                          5.XG Boost classifier.
                          
                          6.KNN Classifier.
                          
15.Checking the feature importance of different models.

                 1.Downvotes.
                 
                 2.Viewcount. 
                 
  These are two important features.

16.Out of all the classifier models KNN classifier gives the best accuracy of 0.87.





3.Wikipedia Article Classification:


Question: Perform a binary classification on feature and non-feature Wikipedia articles.



Details: Provided a repository of Wikipedia articles, your task is to create a binary classification
model to classify the articles as featured and non featured.



SOLUTION:
STEPS INVOLVED IN THIS PROJECT:

1.Importing the required libraries.


2.Import the dataset.We have to use delimiter to remove the delimiters.

3.The given data is an csv file, we use it only for labelling the articles as Featured or Non featured.

4.The dataset consists of more than 6.5 million articles we do random sampling and only take the limited amount of data.


5.After extracting the data we have to extract the features from the data using the Wikipedia Api.

                1.Text length of Article.
                
                2.Title length.
                
                3.Section count.
                
                4.Category count.
                
                5.No of external links.
                
                6.Class.
                
                7.Article name
          
6.The target variable is created from the class column in the dataset.We have to create a feature matrix with all the features.


7.It is a Binary class classification problem,so it is necessary to check whether target variable is balanced or not.


8.DATA CLEANING:

             1.Checking for the null values.
             
             2.Spelling correction in the columns.
             
             3.Checking the datatypes.
             
             4.Checking for duplicates.
             
             5.Checking for outliers.
             
             
             
9.Explanatory Data Analysis:

             1.Distribution  of features.
             
             2.Feature vs Target.
             
10.Using correlation matrix to find the correlation between features.

11.Encoding the data.

12.Target and Feature selection.

13.Target variable is imbalanced,so we are using some of the data balancing techniques
                       
                       1.SMOTE.
                       
                       2.SMOTENN.
                       
Out of theses SMOTENN gives best accuracy.

14.Splitting the model into train and test.

15.Fitting the data with different classifier models.

                          1.Logistic Regression.
                          
                          2.Random Forest Classifier.
                          
                          3.Decision Tree classifier.
                       
                          4.XG Boost classifier.
                          
                          5.SVM Classifier.
                          
16.Checking the feature importance of different models.

                 1.Text length
                 
                 2.Section count.
                 
  These are two important features.

17.Out of all the classifier models SVM classifier gives the best accuracy of 0.95.

18.The wikipedia Article classifcation gives this much accuracy with only one feautre. i.e: Text length .

