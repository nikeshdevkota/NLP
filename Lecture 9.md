# Natural Language Processing
## Lesson 9

<h3> Transformers</h3>

* Transformers were introduced in a 2017 research paper by Google researchers and quickly became the state-of-the-art approach for many natural language processing tasks.
* They replaced the previous dominant approach, recurrent neural networks (RNNs), which had limitations in processing long sequences of text.
* The key innovation of transformers is the attention mechanism, which allows the model to selectively focus on different parts of the input sequence when processing each token. 
* This attention mechanism enables the transformer to capture the relationships between different parts of the input sequence and has greatly improved the performance of natural language processing tasks.

<h3>Transformer Architecture</h3>

* Transformers consist of an encoder and a decoder. 
* The encoder processes the input sequence and generates a representation that captures the meaning of the text. 
* The decoder uses the encoder's representation to generate the output sequence, such as a translation or a summary.


<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/222999525-a4a98828-8e77-4146-9aab-cedc501fb297.svg" width="550" title="Transformers">
</p>

<h4> Encoder </h4>

* The input (source) and output (target) sequence embeddings are added with positional encoding before being fed into the encoder and the decoder that stack modules based on self-attention.
* Transformer encoder is a stack of multiple identical layers, where each layer has two sublayers.
* The first is a multi-head self-attention pooling and the second is a positionwise feed-forward network.
* Specifically, in the encoder self-attention, queries, keys, and values are all from the outputs of the previous encoder layer. 
*  Inspired by the ResNet, a residual connection is employed around both sublayers. 

<h4> Decoder </h4>

* The Transformer decoder is also a stack of multiple identical layers with residual connections and layer normalizations. 
* Besides the two sublayers described in the encoder, the decoder inserts a third sublayer, known as the encoder-decoder attention, between these two. 
* In the encoder-decoder attention, queries are from the outputs of the previous decoder layer, and the keys and values are from the Transformer encoder outputs. 
*  In the decoder self-attention, queries, keys, and values are all from the outputs of the previous decoder layer. 
*  However, each position in the decoder is allowed to only attend to all positions in the decoder up to that position.
*  This masked attention preserves the auto-regressive property, ensuring that the prediction only depends on those output tokens that have been generated.

