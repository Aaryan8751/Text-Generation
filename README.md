# Text-Generation
Build a Neural Network based model to predict what the next word will be in a sequence of words/sentences.

## Background
The text generation problem took some time to solve and perfect. Unlike images, dealing with text and natural language needs some temporal memory because human languages contain various subtleties. A simple example is the use of pronouns like he, she, or it instead of nouns, like somebody's name. These things are just _understood_ by humans but machines need to learn which name can be replaced by "she" and when. This is done using RNNs - a class of neural nets used for many language tasks. Their specialty lies in a mechanism that helps them retain bits of information to use later. The LSTM unit is a kind of RNN and was one of the most popular tools for natural language processing before transformers emerged.

## Dataset
The dataset is taken from [Gutenberg](https://www.gutenberg.org/). [Here](https://www.gutenberg.org/files/1661/1661-0.txt) is the dataset. The dataset consists of The Adventures of Sherlock Holmes, by Arthur Conan Doyle to train my model.

## Code Information
We have used Keras Sequential model to train the model with categorical_crossentropy as the loss function and adam as the optimizer. Embedding, Bidirectional, LSTM, and Dense layers are used in this model. Early Stopping is used to stop early when the accuracy is not increasing much. To convert text into sequences we have used Keras Tokenizer and pad_sequences.

## Prerequisites
You need to have installed the following software and libraries on your machine before running this project.
1. Python 3
2. Anaconda: It will install an ipython notebook and most of the libraries which are needed like sklearn, pandas, seaborn, matplotlib, numpy, PIL.
3. TensorFlow
4. Keras
## Installing
1. Python 3: https://www.python.org/downloads/
2. Anaconda: https://www.anaconda.com/download/
3. Tensorflow: pip install tensorflow
4. Keras: pip install keras
