# Natural Language Processing
## Lesson 1

<h3> Bags of Words </h3>

* Bags of words is a simple representation of text data in NLP. 
* The idea is to convert a text document into a numerical vector by counting the occurrences of words in the document.
* Each unique word in the corpus is assigned a unique index and a document is represented as a vector of the word count values.
* This representation ignores the order of words and the context in which they appear.
* Bags of words is commonly used as a preprocessing step for various NLP tasks, including text classification, clustering, and information retrieval, but it has limited ability to capture the meaning of words and the relationships between words.

<h3> Word2vec algorithm family </h3> The Word2Vec algorithm family consists of two variants: Continuous Bag-of-Words (CBOW) and Skip-gram.

* Continuous Bag-of-Words (CBOW): The CBOW model predicts the target word based on its surrounding context words. The input to the model is a context window of surrounding words, and the output is the target word in the center of the window. CBOW uses a shallow neural network with a single hidden layer to learn the word vectors. The hidden layer is trained to predict the target word based on the context words, using a negative sampling technique to approximate the probability distribution of the target words. The training process adjusts the weights of the network such that the dot product of the word vectors approximates the predicted target word.

* Skip-gram: The Skip-gram model predicts the surrounding context words based on a target word. The input to the model is a target word, and the output is the surrounding context words in the window. The Skip-gram model has been shown to be effective in learning meaningful word vector representations that capture the semantic and syntactic relationships between words. Compared to the CBOW variant, the Skip-gram model is computationally more efficient and may perform better on smaller text corpora. However, it requires more memory, as it generates multiple predictions for each input word.
