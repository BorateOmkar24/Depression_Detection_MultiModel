👋 Introduction

This project focuses on detecting suicide ideation in text data using various machine learning and deep learning models. The dataset consists of Reddit posts from the "SuicideWatch" and "depression" subreddits, labeled as "suicide" or "non-suicide." Our goal is to classify posts based on the presence of suicide ideation, leveraging different models for text classification and comparing their performance.

📖 Dataset

The dataset includes Reddit posts from the "SuicideWatch," "depression," and "r/teenagers" subreddits. Posts from "SuicideWatch" are labeled as suicide, while non-suicide posts are collected from "r/teenagers." The dataset was collected using the Pushshift API, covering:

"SuicideWatch" posts from Dec 16, 2008, to Jan 2, 2021. "depression" posts from Jan 1, 2009, to Jan 2, 2021. This dataset is designed to assist with suicide detection models in text classification tasks.

https://www.kaggle.com/datasets/nikhileswarkomati/suicide-watch

🥷 Models

1. Naive Bayes (Baseline)
This is our baseline model, serving as a reference point for performance comparison. It’s simple and effective, typically used for text classification tasks.

2. Feed-forward Neural Network (Dense Model)
A simple dense model (fully connected layers) that learns patterns in the input data to make predictions. It's designed to capture complex relationships within the data.

3. Long Short-Term Memory (LSTM) Model (RNN)
LSTM is a specialized Recurrent Neural Network (RNN) that can capture long-range dependencies and overcome the vanishing gradient problem, making it ideal for sequential data like text.

4. Gated Recurrent Unit (GRU) Model (RNN)
GRU is another type of RNN similar to LSTM but with a simplified architecture. It can model sequential data while being computationally more efficient than LSTM.

5. Bidirectional LSTM Model (RNN)
Bidirectional LSTM processes input sequences in both forward and backward directions, allowing it to capture more context and improve accuracy.

6. 1D Convolutional Neural Network (CNN)
CNN is used to detect patterns in the text by extracting features at different levels, which can be particularly useful in classifying short text sequences.

7. TensorFlow Hub Pretrained Feature Extractor (Transfer Learning for NLP)
This model uses transfer learning, leveraging a pre-trained text embedding model from TensorFlow Hub to classify the text. It offers the advantage of using knowledge learned from a large dataset to improve classification performance.

Ensemble Model
The ensemble model combines predictions from multiple models using techniques like stacking to improve overall performance and accuracy.

