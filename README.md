# Wine-variety
Welcome to this Repo
I was not able to upload the train and test csv because it was too large. Predicting variety of wine based on country, review_title, review_description, designation, province, region_1, winery, year. 

Step 1) Open train_model.ipynb/train_with_kfold.ipynb and change the location of train and test csv as you've kept in your directory.

Step 2) Run train_model.ipynb/train_with_kfold.ipynb, You'll get a prediction_for_testcsv which has all the predictions for the test data.

Accuracy: 96%
So for this model I used NLP and neural networks to make the model. I'll describe the things that I did sequentially.
1) Loaded the data.
2) Used re module to extract years from the review_title and appended into train dataframe.
3) Removed the rows which didnt have years.
4) Added blank space where ever no values were present in the train dataframe.
5) Joined the columns (country, review_title, review_description, designation, province, region_1, winery, year) and made a new column that contained all these.
6) Removed the stopwords but kept the year as string.
7) Used TFIDF vectorization for this 'new' column. 
8) Extracted variety column and stored in variable.
9) Made model from dense layers.
10) Fitted the model and predicted the test cases.

Features used = country, review_title, review_description, designation, province, region_1, winery, year.
Insigths from data: 1)A lot of wines are from 83 to 93 points.
                    2)England and Austria are at the top pointer countries.
                    3)Switzerland and England rank high for expensive wines.
                    4)9 people rated 'Bordeaux-style Red Blend' above 99 points.
                    5)US is at the top of the list in number of wines produced.
                    ALL THESE INSIGHTS ARE PLOTTED IN 'visualizatioon.ipynb'.



