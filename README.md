# classifying-disaster-tweets

## Project Overview
A Python project utilizing LSTMS, GRUs and BERT based models to classify if a tweet was about a disaster or not. The data is from a Kaggle competition (https://www.kaggle.com/competitions/nlp-getting-started) and contains 10k+ tweets with the following columns:

1. Text : Main content of tweet
2. Target : Binary label indicating the disaster ( 1 or 0)
3. Keywords : Important words extracted from a tweet
4. Location : Geographical Information

The training data is present train.csv, and the test data is present in test.csv.

This was built using using Python (Keras and Tensorflow).

## Code

Our three main approaches were as follows:

1. An Ensemble model with LSTMs and GRUs (code present in mgmt590_final_project_layer_normalization.ipynb)
2. An Ensmeble model with LSTMs and GRUs but using Word2Vec as the embedding layer (code present in mgmt590_final_word2vec.ipynb)
3. A BERT based model (distilBERT) (code present in mgmt590_final_project_distilbert_with_validation.ipynb)

The best performing one was the distilBERT model, but unfortunately we did not have the resources or the time to improve its performance. With data augmentation and ensembling, the results can be further improved. More details on the models and our findings can be found in the ML Project Presentation deck.
