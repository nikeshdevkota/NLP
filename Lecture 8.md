# Natural Language Processing
## Lesson 7

<h3>Problems with RNN </h3>

* Vanishing Gradient Problem: RNNs are trained using backpropagation, where the error signal is propagated backwards through the network to adjust the weights. However, this process can lead to the gradients becoming very small as they are propagated backwards through time, which can make it difficult for the network to learn long-term dependencies.

* Exploding Gradient Problem: On the other hand, in some cases, gradients can also become very large, which can cause the weights to explode and the network to become unstable.

* Short-term Memory: RNNs have a short-term memory, which means they can struggle to remember information that was presented more than a few time steps ago. This can make it difficult for them to learn tasks that require long-term memory, such as understanding the context of a longer text.

* Sequential Processing: RNNs process input sequences sequentially, which means they have to wait for each time step to complete before moving on to the next. This can make them slow to process long sequences of data, especially if there are dependencies between different parts of the sequence.

* Difficulty with Parallelization: RNNs are difficult to parallelize, which can make them slower to train on large datasets.

<h3>Problems with LSTM </h3>

Despite being good at capturing long-term dependencies, LSTM networks also can still have difficulty in processing and understanding very long sequences, as the model may lose track of important information from the beginning of the sequence.

<h3> Attention </h3>


Attention mechanism is one of the recent advancements in Deep learning especially for Natural language processing tasks like Machine translation, Image Captioning, dialogue generation etc. 

Attention mechanism in Natural Language Processing (NLP) is a technique used to enable a model to selectively focus 
on specific parts of the input sequence when processing it. The goal of attention is to improve the quality of the output by
giving the model the ability to weigh the importance of each part of the input sequence when generating the output.

In NLP, attention is often used in conjunction with recurrent neural networks (RNNs) or transformers, which are popular deep learning models used for processing sequential data such as text. Attention enables the model to selectively attend to different parts of the input sequence, allowing it to better understand the context and meaning of the input text.

The attention mechanism works by computing a set of attention weights for each token in the input sequence, which represent the importance of that token relative to the other tokens in the sequence. These attention weights are then used to compute a weighted sum of the input sequence, which is used as input to the next layer of the model.

There are several types of attention mechanisms used in NLP, including additive attention, multiplicative attention, and self-attention. Additive attention involves computing a weighted sum of the input sequence using a learned weight matrix, while multiplicative attention involves computing the attention weights as a dot product between the input sequence and a learned weight matrix. Self-attention, also known as transformer attention, involves computing attention weights between different positions in the input sequence, enabling the model to attend to the most relevant parts of the input at each step of processing.

Overall, attention mechanisms have proven to be a powerful tool in NLP, enabling models to achieve state-of-the-art results on a wide range of tasks, including machine translation, language modeling, and text classification.

