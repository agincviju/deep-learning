1. Aim

To implement and compare different Recurrent Neural Network (RNN)-based models (SimpleRNN, LSTM, and GRU) for text classification on the IMDB movie reviews dataset.

2. Problem Statement

Build and evaluate deep learning models for sentiment analysis of movie reviews, classifying them as positive or negative.

3. Deep Learning Methods & Description

SimpleRNN
A basic recurrent neural network that processes sequences but suffers from vanishing gradient problems on long sequences.

LSTM (Long Short-Term Memory)
An advanced RNN variant that uses memory cells and gates (input, forget, output) to capture long-term dependencies in text.

GRU (Gated Recurrent Unit)
A simplified LSTM that uses fewer gates (reset and update) but performs comparably with faster training.

All models are built using Keras with an Embedding layer for word representations, followed by the chosen recurrent layer and a Dense layer with sigmoid activation for binary classification.

4. Methods Applied to Solve the Problem

Data Preprocessing

Load IMDB dataset with top 10,000 frequent words.

Pad sequences to a maximum length of 500 for uniform input.

Model Training

Implemented three models: SimpleRNN, LSTM, and GRU.

Used Adam optimizer, binary cross-entropy loss, batch size of 64, and 10 epochs.

Model Evaluation

Accuracy measured on test data.

Compared validation accuracy and loss trends.

5. Results

SimpleRNN: Achieved ~78–80% validation accuracy but showed signs of overfitting (training accuracy → 99%, validation stagnates).

LSTM: Achieved ~84–87% test accuracy, more stable performance.

GRU: Similar to LSTM, with ~83–85% accuracy and slightly faster training.

Example outcome:

Final Test Accuracy: ~83–85% (best with LSTM/GRU).

6. Conclusion

RNN-based models effectively classify text sentiment in the IMDB dataset.

LSTM and GRU outperform SimpleRNN by better handling long-term dependencies.

GRU is preferred when faster training is needed, while LSTM is slightly more robust.

This experiment shows the importance of recurrent architectures for NLP tasks.
