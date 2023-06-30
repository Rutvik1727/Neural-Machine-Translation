# Sequence-to-Sequence Translation using RNN
This repository contains an implementation of sequence-to-sequence (Seq2Seq) translation using Recurrent Neural Networks (RNN). The Seq2Seq model is a popular approach for tasks such as machine translation. The model is implemented in PyTorch and can be used to translate between any two languages.

## Model Architecture
The Seq2Seq model consists of two main components: an Encoder and a Decoder.

## Encoder
The encoder takes the input sequence and transforms it into a fixed-size vector called the context vector. In this implementation, the encoder is built using a recurrent neural network, specifically a Long Short-Term Memory (LSTM). The encoder processes the input sequence step by step and updates its hidden state at each time step. The final hidden state of the encoder serves as the context vector.

## Decoder
The decoder takes the context vector produced by the encoder and generates the output sequence word by word. Like the encoder, the decoder is also an RNN, usually an LSTM. It initializes its hidden state with the context vector and generates the output sequence one word at a time. The decoder continues generating words until an end-of-sequence token is produced or a predefined maximum length is reached.

## Training
The training process involves feeding pairs of input sequences and target sequences to the model. The model learns to minimize the difference between its predicted output and the target output.

## Graphs

### Loss
![](https://github.com/Rutvik1727/Neural-Machine-Translation/blob/main/Seq2Seq/Images/plt%20(2).png)

### Perplexity
![](https://github.com/Rutvik1727/Neural-Machine-Translation/blob/main/Seq2Seq/Images/plt%20(1).png)

## Results
> Obtained a BELU score of 28.45

> Obtained a Perplexity of 15%