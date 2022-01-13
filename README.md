# Using reddit posts as a predictor for future stock price growth

The code is structured in the following order:

1: ETL process, part 1: Download and Unzip dataset, explore and use NER to find posts that discuss a certain stock listed. 

2: Download matching stock prices for the current year and process the data. A tiny bit of visualizations of the dataset

3: Use NLTK Vader and FinBERT to perform sentiment analysis of the stocks

4: Evaluate the possibility of predicting stock price movements with a moving average sentiment score based on the two models used in 3.

5: Combine the sentiment scores with document (and title) embeddings for each post to create a large dataset that will be used by the classifier

6: Evaluate several classifiers on several subsets of the dataset (one evaluation per stock and subreddit)

If you wish to view the code for each of the steps, simply look at the jupyter notebook with the correct number (1-6)

A complete list of evaluation results can be found in "processed_results.xlsx"