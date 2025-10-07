SHALLOW AUTO ENCODER AND DECODER NETWORK FOR MACHINE TRANSLATION
AIM:
To implement a shallow auto encoder and decoder network for machine translation(by using Kaggle English to Hindi neural translation dataset). 

2. Problem Statement

Design and evaluate an RNN-based Encoder–Decoder model capable of accurately translating input text sequences into target language sequences after appropriate preprocessing and tokenization steps.

3. Deep Learning Method & Description

This experiment demonstrates how a Sequence-to-Sequence Recurrent Neural Network (Seq2Seq RNN) can be applied to machine translation tasks.

Model Used: Encoder–Decoder RNN with LSTM units

Description:
The Seq2Seq model consists of two main parts:

Encoder: Reads and encodes the input text sequence into a fixed-length context vector.

Decoder: Takes this context vector and generates the output sequence step by step.
The Long Short-Term Memory (LSTM) layers help the model remember long dependencies between words, making it well-suited for language translation.

4. Methods Applied to Solve the Problem

a) Data Preprocessing

Collected paired text samples (input–target).

Performed tokenization, vocabulary creation, and sequence padding.

Converted all words into integer sequences for training.

b) Model Training

Implemented an encoder-decoder architecture using Embedding and LSTM layers.

Compiled the model with Adam optimizer and sparse_categorical_crossentropy loss.

Trained for 10 epochs using a batch size of 64.

c) Model Evaluation

Accuracy and loss were measured for each epoch.

Model performance was evaluated by observing improvements in translation accuracy and reduction in loss across epochs.

5. Results

The model achieved approximately 64.25% accuracy after 10 epochs of training.

Loss decreased steadily from 3.16 to 1.29, indicating improved learning performance.

The results confirm that the RNN-based Seq2Seq model effectively learned sequence mapping between input and target languages.

Training Summary:

Epoch	Accuracy	Loss
1	     0.00	    3.16
5	     0.43	   2.03
10	  0.64   	1.29
6. Conclusion

The Recurrent Neural Network (Seq2Seq) model provided an effective solution for the text translation task. It successfully learned to map input text sequences to target sequences with satisfactory accuracy. The experiment demonstrates the potential of RNNs for natural language processing tasks such as translation, summarization, and question answering.

Future improvements can include using attention mechanisms or transformer-based architectures (like BERT or GPT) to enhance accuracy and context understanding.
