# Natural Language Processing
## Lesson 4

Humans communicate complex ideas by composing words together into bigger units to convey complex meanings. A model needs to understand sentence structure in order to be able to interpret language correctly

<h3> Phase Structure Grammar </h3>

* Phrase structure refers to the way words and phrases are organized in a sentence to form a syntactic structure. 
* It includes the rules for combining words into larger units, such as noun phrases, verb phrases, and adjective phrases, which then combine to form the sentence as a whole. 
* In linguistic theory, phrase structure is represented using tree diagrams that show the hierarchical relationship between the constituent elements of a sentence.
* In PSG, a sentence is represented as a tree structure, with the root node representing the sentence as a whole, and other nodes representing smaller units, such as noun phrases, verb phrases, and adjective phrases. 
* The rules of PSG specify how these phrases can be combined to form a sentence, and how the constituent elements of a phrase are related to each other.


<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/215659075-4cda115f-1dd5-49c6-9712-3251e8cc134e.PNG" width="350" title="Whales">
</p>

<h3> Dependency Grammar </h3>

* Dependency Grammar is a type of grammar that describes the relationships between words in a sentence. 
* Unlike phrase structure grammar, which focuses on grouping words into constituents, dependency grammar focuses on the relationships between individual words and how they depend on each other to form the sentence as a whole.
* In a dependency grammar, each word in a sentence is treated as a node in a graph, with directed edges representing the relationships between words.
* The relationships are typically labeled with grammatical relations, such as subject, object, or modifier. 
* The result is a directed acyclic graph (DAG) that captures the relationships between words in a sentence.

Dependency grammar has several advantages over phrase structure grammar, including its ability to handle complex sentence structures and its simplicity in modeling linguistic phenomena. Dependency grammar is widely used in NLP applications, such as parsing and information extraction, and is particularly useful for languages with free word order, where the relationships between words are more important than their linear order.

<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/215660338-3ea9890b-b9eb-4651-9b6e-5d8b20014832.PNG" width="350" title="Dependency Grammar">
</p>

<h3> Dependency Parsing </h3>

* Dependency Parsing is the process of analyzing the relationships between words in a sentence to identify the dependencies between them.
* The goal of dependency parsing is to build a directed acyclic graph (DAG) that captures the relationships between words in a sentence.
* In a dependency parse, each word in a sentence is represented as a node in the graph, with directed edges representing the relationships between words. 
* The relationships are typically labeled with grammatical relations, such as subject, object, or modifier.
* The result is a graph that captures the relationships between words in a sentence and provides a structural representation of the sentence.
* Dependency parsing is widely used in NLP for tasks such as information extraction, machine translation, and text classification. 
* It is particularly useful for handling languages with free word order, where the relationships between words are more important than their linear order.
* There are several algorithms for performing dependency parsing, including transition-based parsing, graph-based parsing, and neural network-based parsing.
* The choice of algorithm depends on the specific requirements of the task and the characteristics of the language being parsed. 
* Regardless of the algorithm used, the output of a dependency parse is a graph that captures the relationships between words in a sentence and provides a structural representation of the sentence.

<h3> Treebanks</h3>

* Treebanks are annotated corpora of text that provide a structural representation of the sentences in the text. 
* Treebanks are widely used in natural language processing (NLP) to train and evaluate NLP models, and to gain insights into the structure and meaning of language.
* In a treebank, each sentence is annotated with a tree structure that represents the syntactic structure of the sentence. 
* The tree structure can be either a constituency tree, which represents the sentence as a hierarchy of constituent phrases, or a dependency tree, which represents the relationships between words in a sentence.
* Treebanks can be annotated with various linguistic annotations, including part-of-speech tags, named entity tags, and coreference information. 
* The annotation scheme used in a treebank depends on the specific requirements of the NLP task and the characteristics of the language being annotated.
* There are several well-known treebanks, including the Penn Treebank, the Lancaster-IBM Treebank, and the Universal Dependencies Treebank. 
* These treebanks have been widely used as benchmark datasets for evaluating NLP models, and have contributed to advances in NLP over the past few decades.

<h3> Projective Parse </h3>

* Projective parse is a type of parse tree used in natural language processing (NLP) to represent the syntactic structure of a sentence. 
* Projective parses are typically represented as directed acyclic graphs (DAGs), where each node in the graph represents a word in the sentence and the edges represent the relationships between the words.
* A projective parse is called projective because it preserves the linear order of the words in the sentence, meaning that if two words appear in a certain order in the sentence, then the corresponding nodes in the parse tree must also be ordered in the same way. 
* This property makes projective parses well-suited for NLP tasks that require the preservation of the original sentence order, such as machine translation.
* Projective parses are often generated using dependency parsing algorithms, which aim to identify the relationships between words in a sentence and construct a graph-based representation of the sentence structure.
* Dependency parsing algorithms typically use information from sources such as part-of-speech (POS) tags, syntactic structure, and lexical information to identify the relationships between words in a sentence.







