# Sentiment Classification with LSTM

## Introduction

LSTM (Long Short-Term Memory) is a type of Recurrent Neural Network (RNN) architecture that is designed to process and predict sequences of data. LSTMs are particularly effective at capturing long-term dependencies in data, addressing a key limitation of traditional RNNs, which often struggle with the problem of "vanishing gradients" and have difficulty retaining information over long sequences.

In a sentiment analysis task, LSTM (Long Short-Term Memory) networks are widely used because they excel at handling sequential data, such as text, where the meaning of a word or sentence often depends on previous words. LSTMs help the model retain context over long sequences, making them highly effective for understanding and predicting the sentiment (positive, negative, neutral) of a given piece of text.

## Dataset

This experiment employs a dataset that comprises movie reviews. The dataset used for model training is publicly available on Kaggle and accessible for free on the internet. The link to this data is [Kaggle Rotten Tomatoes EDA](https://www.kaggle.com/code/stefanoleone992/rotten-tomatoes-eda). The movie reviews were annotated using [RoBERTa](https://github.com/bitacode/Labeling-Dataset-For-Sentiment-Analysis.git).

## Results

The LSTM model achieved a training accuracy of 80.87% and a validation accuracy of 80.84% indicating that the model performs well on both the training and validation datasets with minimal overfitting. The training loss of 0.5558 and validation loss of 0.5587 are also closely aligned, suggesting that the model has generalized well to unseen data.

The LSTM model achieved an overall accuracy of 81% on the sentiment analysis task, with the highest performance observed in the positive class, achieving an F1-score of 0.86 and a recall of 0.88. The model also performed equally well on the negative class, with an F1-score of 0.84. However, the model's performance was slightly lower on the neutral class, with an F1-score of 0.72 and a recall of 0.70, suggesting some difficulty in distinguishing neutral sentiment. The macro average and weighted average F1-scores are both 0.81, indicating consistent performance across all classes, with no significant bias towards any particular class. Overall, the model demonstrates strong predictive capabilities but could benefit from further fine-tuning, particularly in improving neutral class predictions.

## Prospects

LSTM is specifically designed for sequential data, making it perform very well in sentiment analysis tasks. However, based on the training results, it's clear that this experiment has the potential to achieve higher performance. Increasing the number of epochs to 100 or more could further improve the results.
