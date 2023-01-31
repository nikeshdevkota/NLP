# Natural Language Processing
## Lesson 6

<h3> Perplexity </h3> 

* Perplexity is a measure of the quality of a language model. 
* It is used to quantify how well the model predicts a given text.
* It is calculated as the exponential of the average negative log-likelihood of the words in the text.
* Perplexity is expressed as a number, and the lower the perplexity score, the better the model is at predicting the text.
* For example, if a model assigns a high probability to the words in a text, then the perplexity score will be low.
* If two models are trained on the same data, the model with the lower perplexity score is considered to be a better fit for the data.


<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/215668503-17a8edab-92d2-4762-88d7-a55f2b66a6da.PNG" width="350" title="Ice Gas">
</p>

<h3> LSTM Networks </h3> 

* LSTM stands for Long Short-Term Memory, and it is a type of recurrent neural network (RNN) used for processing sequential data, such as text, speech, or time series data.
* In traditional RNNs, the network has a hidden state that is updated at each time step, based on the input and the previous hidden state. 
* However, traditional RNNs have difficulty preserving information over long sequences, due to the vanishing gradient problem.
* LSTMs were designed to overcome this issue by introducing a memory cell that can store information over a long period of time, and gates that control the flow of information into and out of the memory cell.
* This allows LSTMs to maintain a much more stable hidden state, even over very long sequences, making them well-suited for tasks that require modeling long-term dependencies, such as language modeling or speech recognition.
