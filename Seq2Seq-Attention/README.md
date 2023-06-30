# Sequence-to-Sequence Translation with Attention Mechanism using RNN
This repository contains an implementation of sequence-to-sequence (Seq2Seq) translation with attention mechanism using Recurrent Neural Networks (RNN). The addition of attention mechanism allows the model to focus on specific parts of the input sequence when generating the output sequence, improving translation accuracy and handling longer sequences more effectively.

## Model Architecture
The Seq2Seq model with attention mechanism extends the basic Seq2Seq model by introducing an attention mechanism between the encoder and decoder.

## Encoder
The encoder takes the input sequence and processes it step by step, just like in the basic Seq2Seq model. It is implemented using GRU. The final hidden state of the encoder is used as the initial hidden state of the decoder.

## Attention Mechanism
The attention mechanism is added between the encoder and decoder to capture the relevant information from the input sequence during the decoding process. It enables the model to focus on different parts of the input sequence at each decoding step.

## Decoder
The decoder generates the output sequence based on the attention mechanism and the hidden state from the encoder. It is also implemented using GRU. At each decoding step, the attention mechanism computes attention weights for different parts of the input sequence, and the decoder combines these weighted representations to make more informed predictions for the next output word.

## Training
The training process for the Seq2Seq model with attention mechanism is similar to the basic Seq2Seq model. Pairs of input sequences and target sequences are fed into the model, and the model learns to minimize the difference between its predicted output and the target output.

## Graphs

### Loss
![](https://github.com/Rutvik1727/Neural-Machine-Translation/blob/main/Seq2Seq-Attention/Images/plt%20(2).png)

### Perplexity
![](https://github.com/Rutvik1727/Neural-Machine-Translation/blob/main/Seq2Seq-Attention/Images/plt%20(1).png)

## Results
> Obtained a BELU score of 30.50

> Obtained a Perplexity of 10%