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

* Skip-gram: The Skip-gram model predicts the surrounding context words based on a target word. The input to the model is a target word, and the output is the surrounding context words in the window. In the negative sampling technique, a small number of negative examples (random words from the vocabulary that are not in the context window) are selected for each input word. The network is trained to predict the context words as positive examples and the negative examples as negative examples. This allows the model to focus on the most informative examples and reduce the number of computations required to train the network.

<h3> Window based Co-occurence Matrix </h3> 

* A window-based co-occurrence matrix is a method of representing the relationship between words in a corpus of text.
* The basic idea is to count the number of times each pair of words co-occur within a fixed-sized window in the text.
* The resulting matrix is a symmetrical square matrix where the rows and columns represent words and the cells represent the number of co-occurrences between pairs of words.

For example, consider the following sentence: "I love dogs and cats". If we use a window size of 1, we would count the number of times each pair of words appears within a distance of 1 word. In this case, we would have the following co-occurrence matrix:

<table><thead><tr><th></th><th>I</th><th>love</th><th>dogs</th><th>and</th><th>cats</th></tr></thead><tbody><tr><td>I</td><td>0</td><td>1</td><td>0</td><td>0</td><td>0</td></tr><tr><td>love</td><td>1</td><td>0</td><td>1</td><td>1</td><td>0</td></tr><tr><td>dogs</td><td>0</td><td>1</td><td>0</td><td>1</td><td>1</td></tr><tr><td>and</td><td>0</td><td>1</td><td>1</td><td>0</td><td>1</td></tr><tr><td>cats</td><td>0</td><td>0</td><td>1</td><td>1</td><td>0</td></tr></tbody></table>


