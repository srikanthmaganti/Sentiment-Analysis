# Sentiment-Analysis
This repository mainly consists of three different folders working on same dataset but in different environments

-----------------------------------------Sentiment Analysis using Pytorch--------------------------------------

This folder consists of ipynb file and saved weights.txt

1.In the initial stage of the model building I have taken preprocessed file because for some reason spacy package preprocessing is not working. So, I have used my own preprocessing techniques to filter the raw data and stored it as pickle file to use in later stages

2.Coverted this into tabular dataset and used TorchText for building vocabulary and used GloVe(100) word embeddings, Hyperparameter Tuning for BilSTM model

3.Trained the model,built an Inference model and predicting sentiment of the given sentences

-----------------------------------------Sentiment Analysis using TensorFlow------------------------------------

This folder consists of 2 ipynb files

Sentiment Analysis using Recurrent Neural Networks and CNN's

1.Preprocessed the raw text data of movie reviews and converting them into word2vec form GloVe word embeddings

2.Training the model,hyperParameter tuning,and evaluating the training accuracy and validation accuracy

3.While working with CNN's, I have acheived an accuracy of 82% 

----------------------------------------Sentiment Analysis in SageMaker------------------------------------------

1. After all the model building is done, I have deployed the model with PyTorch in production environment

2.The End point of model inference which was deployed is given in the Lambda function for internal access

3.Built a UI website for users whcich it goes to lambda function and from lambda function to End point where model inference is residing and computation is done over there and the result is sent back to UI 
