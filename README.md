# Next Word Predictor
This project involves building a Next Word Predictor using a Kaggle dataset. The model predicts the next word in a sentence based on the given input. The project leverages deep learning techniques, including Tokenizer for word processing and LSTM layers for sequential data prediction.

## Project Description
Data Preprocessing
### Tokenizer:

Used the Tokenizer class to create key-value pairs of words in the dataset.
Converted the text data into sequences of integers.
### Sequence Padding:

Applied padding to ensure that all sequences have the same length, which is necessary for training the LSTM model.
## Model Building
### Embedding Layer:

Utilized an Embedding layer to convert integer sequences into dense vectors of fixed size.
This layer helps in capturing the semantic meaning of words by representing them in a high-dimensional space.
### LSTM Layer:

Implemented Bidirectional LSTM (Long Short-Term Memory) layer to handle the sequential nature of the text data.
LSTM is effective in learning long-term dependencies, which is crucial for predicting the next word based on previous words in a sentence.
### Dense Layer:

Added a Dense layer with a softmax activation function to output the probability distribution over the vocabulary for the next word prediction.
## Model Training
### Compilation:

Compiled the model using the Adam optimizer and sparse_categorical cross-entropy loss function.
### Metrics used: Accuracy
## Training:

Trained the model on the dataset with a specified number of epochs and batch size.
Used validation data to monitor the model's performance and avoid overfitting.
