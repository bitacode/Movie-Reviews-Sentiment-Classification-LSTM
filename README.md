# Sentiment Classification with LSTM

## Introduction

LSTM (Long Short-Term Memory) is a type of Recurrent Neural Network (RNN) architecture that is designed to process and predict sequences of data. LSTMs are particularly effective at capturing long-term dependencies in data, addressing a key limitation of traditional RNNs, which often struggle with the problem of "vanishing gradients" and have difficulty retaining information over long sequences.

In a sentiment analysis task, LSTM (Long Short-Term Memory) networks are widely used because they excel at handling sequential data, such as text, where the meaning of a word or sentence often depends on previous words. LSTMs help the model retain context over long sequences, making them highly effective for understanding and predicting the sentiment (positive, negative, neutral) of a given piece of text.

## Dataset

This experiment employs a dataset that comprises movie reviews. The dataset used for model training is publicly available on Kaggle and accessible for free on the internet. The link to this data is [Kaggle Rotten Tomatoes EDA](https://www.kaggle.com/code/stefanoleone992/rotten-tomatoes-eda). The movie reviews were annotated using [RoBERTa](https://github.com/bitacode/Labeling-Dataset-For-Sentiment-Analysis.git).

## Results

The LSTM model training results show a training loss of 0.5944 and training accuracy of 0.7813, indicating that the model performs reasonably well on the training data, classifying around 78% of the data correctly. On the validation set, the model achieved a slightly better validation loss of 0.5657 and validation accuracy of 0.7948, which suggests that the model is generalizing well to unseen data and not overfitting, with validation performance slightly higher than training performance.

The LSTM model achieved an overall accuracy of 79%. The model performed well in classifying positive and negative sentiments, with both achieving a precision and recall of 0.83, and F1-scores of 0.85 and 0.83 respectively. However, the model struggled more with the neutral sentiment, where the F1-score was lower at 0.70, reflecting a slightly reduced ability to correctly identify neutral sentiment compared to positive and negative. The macro and weighted averages for precision, recall, and F1-score are all 0.79, indicating balanced overall performance but room for improvement, particularly in the neutral class.

## Prospects

LSTM is specifically designed for sequential data, making it perform very well in sentiment analysis tasks. However, based on the training results, it's clear that this experiment has the potential to achieve higher performance. Increasing the number of epochs to 100 or more could further improve the results.
