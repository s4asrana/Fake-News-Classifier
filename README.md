# Fake-News-Classifier

This project tries to identify the fake news out of a bunch of news using LSTM's which is a deep learning technique. 

The dataset used is from Kaggle and has around 20000 rows and 5 columns. 
The columns are as follows:

#Id                                                                                                                                                          #Title: Headline of the news article.
#Author 
#Text: Content of the news
#Label: 1-Fake news
        0-Not a fake news
        
It is a classificaton task. The target variable is Label and the independent variables are the remaining four.

For this project I used Long short term memory(LSTMs) which are an updated version of recurrent neural networks(RNNs). RNNs are special architectures that take into account temporal information, which is extremely important for natural language processing, as in NLP the input data does not have a fixed size, and the next word is highly dependent on previous words. Context is very important in NLP.

But RNNs suffer from short-term memory problem and because of this LSTM’s were created. They have internal mechanisms called gates that can regulate the flow of information. These gates can learn which data in a sequence is important to keep or throw away. By doing that, it can pass relevant information down the long chain of sequences to make predictions.

WorkFlow of the task:

1: Data reading using pandas library.
2: Data preprocessing and cleaning like finding and handling null and missing values.
3: Transforming data using tokenization, Stemming, WordEmbedding etc. so that it can be fed to the deep learning model and doing train-test split.
4. Creating deep learning model and fitting it on the training data.
5. Evaluatig model using Classsification accuracy on the test data(The model achieved an accuracy of around 90%).
