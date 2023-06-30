# Neural Machine Translation using Transformers
This repository contains an implementation of machine translation using Transformers, a state-of-the-art architecture for various natural language processing tasks, including machine translation. Transformers have revolutionized the field by providing improved translation accuracy and scalability.

## Model Architecture
The translation model based on Transformers consists of an encoder and a decoder.

## Encoder
The encoder processes the input sequence and generates a sequence of hidden states. Each hidden state captures the contextual information of a specific word in the input sequence. Transformers employ self-attention mechanism within the encoder, allowing the model to consider the entire input sequence simultaneously and capture dependencies efficiently.

## Decoder
The decoder takes the hidden states produced by the encoder and generates the output sequence. Similar to the encoder, it utilizes self-attention mechanism to attend to different parts of the input sequence. Additionally, the decoder employs encoder-decoder cross attention, which helps it align the source and target sequences effectively during translation.

## Training
The training process involves feeding pairs of source sequences and target sequences to the model. The model learns to minimize the discrepancy between its predicted output and the target output.

## Graphs

### Loss
![](https://github.com/Rutvik1727/Neural-Machine-Translation/blob/main/Transformers/Images/plt%20(1).png)

### Perplexity
![](https://github.com/Rutvik1727/Neural-Machine-Translation/blob/main/Transformers/Images/plt%20(2).png)

## Results
> Obtained a BELU score of 38.75

> Obtained a Perplexity of 7%