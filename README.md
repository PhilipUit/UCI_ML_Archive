# UCI_ML_Archive
- We will use a data set from the Bank Marketing data set from the UCI ML Archive (http://archive.ics.uci.edu/ml/datasets/Bank+Marketing).  

Find an "interesting" data set to work with. UCI Machine Learning Archive is a good place to start. After reading the data set's description and looking at the data, propose an "Analysis Question" -- In other words, what is all of your work trying to prove? Clean the data as we have been Missing values Data types String manipulation Wide vs. long format etc. Do feature analysis using Seaborn and Matplotlib to determine which ones are important. Remember to explain your steps. Why are you doing the graph and what did you learn from it? Use a linear model from this weeks' reading. Be sure to split the data into train and test sets. Perform checks on the model's output of the test data. Evaluate accuracy of the model. Final analysis of the results: What was the answer to your Analysis Question? How accurate was the model? Thoughts to improve accuracy? Lessons learned. Deliverable will be the Jupyter notebook and data set."
About the Dataset:

I found this dataset to be intersting personally, as I am naturally curious about market finance, and this was the most detailed dataset about stocks specifically. The data is from: Dr. Michael Brown, michael.brown '@' umuc.edu, University of Maryland University College.

"In predicting stock prices you collect data over some period of time - day, week, month, etc. But you cannot take advantage of data from a time period until the next increment of the time period. For example, assume you collect data daily. When Monday is over you have all of the data for that day. However you can invest on Monday, because you don't get the data until the end of the day. You can use the data from Monday to invest on Tuesday.

In our research each record (row) is data for a week. Each record also has the percentage of return that stock has in the following week (percent_change_next_weeks_price). Ideally, you want to determine which stock will produce the greatest rate of return in the following week. This can help you train and test your algorithm.

Some of these attributes might not be use used in your research. They were originally added to our database to perform calculations. (Brown, Pelosi & Dirska, 2013) used percent_change_price, percent_change_volume_over_last_wk, days_to_next_dividend, and percent_return_next_dividend. We left the other attributes in the dataset in case you wanted to use any of them. Of course what you want to maximize is percent_change_next_weeks_price.

Training data vs Test data: In (Brown, Pelosi & Dirska, 2013) we used quarter 1 (Jan-Mar) data for training and quarter 2 (Apr-Jun) data for testing.

Interesting data points: If you use quarter 2 data for testing, you will notice something interesting in the week ending 5/27/2011 every Dow Jones Index stock lost money"
"Analysis_Question"-- In other words, what is all of your work trying to prove?

The purpose of this lab is to use models to look for relationships between observed features and their outcomes. Based on the content of the dataset, it would be intersting to see if there is any sort of correlation between some cruicial variables in this dataset. At first glance, this is a pretty basic dataset, but after running the dataset through some of the methods we will demonstrate, we will look to find unique observations in the dataset. We will look to aggregate some information by unique stock, look to find correlation in the dataset that could lead to uniique understanding or deeper analysis, and also we will hope to uncover information that could possibly lead to future understandings/correlations by training data and test sets to look for unique inear regression models. Potentially we will discover something groundbreaking and will lead to learning events from the past that can elude to future events occuring? We will see! We will primarily look at volume and it's affect on other variables.

- We will use a data set from the Bank Marketing data set from the UCI ML Archive (http://archive.ics.uci.edu/ml/datasets/Bank+Marketing).  


The data set has 20 feature columns plus one result column and we need to do some work to get it ready for further processing.  1. Reference the bank-additional-names.txt file for column types and what the names mean.  2. Make the following changes: Change column names to remove abbreviations, capitalize, add spaces, and generally make the names more "meaningful" to casual readers. Change column types to match the associated feature types. Replace word separators in strings like "-" or "." with spaces. 3. Missing Attribute Values: There are several missing values in some categorical attributes, all coded with the "unknown" label. These missing values can be treated as a possible class label or using deletion or imputation techniques.
uses data(do see attachment) from the Bank Marketing data set from the UCI ML Archive (http://archive.ics.uci.edu/ml/datasets/Bank+Marketing).

The data set has 20 feature columns plus one result column and we need to do some work to get it ready for further processing.

1
### Reference the bank-additional-names.txt file for column types and what the names mean.

2
### Make the following changes:

- Change column names to remove abbreviations, capitalize, add spaces, and generally make the names more "meaningful" to casual readers.
- Change column types to match the associated feature types.
- Replace word separators in strings like "-" or "." with spaces.
- Do any values need to be replaced with NaN or are they better the way they are?
- #8 in the text file states?

3
### Missing Attribute Values: There are several missing values in some categorical attributes, all coded with the "unknown" label. These missing values can be treated as a possible class label or using deletion or imputation techniques.

- Decide what to do with these "unknown" values and defend your decision.

