# Natural Language Processin
## Lesson 1

<h3>Word Vector</h3> 


* Word vectors are mathematical representations of words used in NLP tasks. 
* They capture the semantic meaning of words by mapping each word to a high-dimensional vector in a continuous vector space, based on the context in which the word appears. 
* Similar words are mapped to vectors that are close together in the vector space, while dissimilar words are farther apart. 
* Word vectors are used in various NLP tasks such as text classification, sentiment analysis, machine translation, etc.

<h3>Examples of Word Vectors</h3> 

* Word2Vec: A popular word vector representation that uses a shallow neural network to learn the relationships between words based on their co-occurrence in large text corpora. The network takes as input a word and predicts the context words that are likely to appear around it. By training the network on multiple context windows, the model can capture the semantic relationships between words, mapping each word to a high-dimensional vector in a continuous vector space. Similar words are mapped to vectors that are close together in the vector space, while dissimilar words are farther apart. This allows Word2Vec to be used in various NLP tasks such as text classification, sentiment analysis, and word analogy.

* GloVe (Global Vectors for Word Representation): Another popular word vector representation that uses a matrix factorization approach to capture the co-occurrence statistics of words in large text corpora. Given a word-word co-occurrence matrix, the goal of GloVe is to learn a word vector representation for each word such that the dot product between two word vectors approximates the logarithm of their co-occurrence count. This approach allows GloVe to capture the semantic and syntactic relationships between words, mapping each word to a high-dimensional vector in a continuous vector space. Similar words are mapped to vectors that are close together in the vector space, while dissimilar words are farther apart. 

