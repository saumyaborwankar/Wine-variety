# Wine-variety
Welcome to this Repo
I was not able to upload the train and test csv because it was too large
Step 1
Open train_model.ipynb and change the location of train and test csv as you've kept in your directory
Step 2 
Run train_model.ipynb, You'll get a prediction_for_testcsv which has all the predictions for the test data

Accuracy: 96%
So for this model I used NLP and neural networks to make the model. I'll describe the things that I did sequentially
1) Loaded the data
2) Used re module to extract years from the review_title and appended into train dataframe
3) Removed the rows which didnt have years
4) Added blank space where ever no values were present in the train dataframe
5) Joined the columns (country, review_title, review_description, designation, province, region_1, winery, year) and made a new column that contained all these
6) Removed the stopwords but kept the year as string
7) Used TFIDF vectorization for this 'new' column 
8) Extracted variety column and stored in variable
9) Made model
10) Fitted the model and predicted the test cases


Predicting variety of wine based on region, review, country, year 

