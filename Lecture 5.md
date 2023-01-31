# Natural Language Processing
## Lesson 5

<h3> Language Modeling </h3>
* Language modeling is the task of predicting the next word in a sequence of words based on the context provided by the preceding words.
* It is a fundamental task in natural language processing (NLP) and is used in a variety of applications, such as speech recognition, machine translation, and text classification.
* Language models are usually trained on large datasets of text, such as books, news articles, or web pages.

<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/215666318-8a6c0908-a361-4949-9075-203f8c022965.PNG">
</p>

* The goal is to learn the probability distribution of words in the language, so that the model can make predictions about the most likely next word given a context.
* Language models can be implemented using a variety of techniques, including n-gram models, hidden Markov models (HMMs), and recurrent neural networks (RNNs).
* More recent approaches to language modeling have focused on using deep neural networks, such as transformer models, which have achieved state-of-the-art results on a variety of language modeling tasks

<h3> Recurrent Neural Networks (RNNs) </h3>

* Recurrent Neural Networks (RNNs) are a type of artificial neural network that are designed to process sequential data, such as text, speech, or time series data. 
* They have a hidden state that is updated at each time step based on both the current input and the previous hidden state, allowing them to maintain information about the context of the input sequence.
* The basic idea behind RNNs is to allow information to flow through the network across time steps.
* At each time step, the hidden state is updated based on the current input and the previous hidden state.
* This allows the network to maintain information about the context of the input sequence and use that information to make predictions about future inputs.

<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/215666692-0b39e123-ca1b-4798-a0ea-16b9a21cb578.PNG">
</p>
