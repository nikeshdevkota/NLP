# Natural Language Processing
## Lesson 15

<h3> Language Models</h3>

Standard language models (LM) predict the next word in a sequence of text and can compute the probability of a sequence.Recently, masked language models (e.g., BERT) instead predict a masked token in a sequence of text using bidirectional context

<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/227144120-740d8dd8-ca84-45db-9b97-b56568943363.PNG" width="550" title="Transformers">
</p>

Traditionally, LMs are used for many tasks involving generating or evaluating the probability of text:
* Summarization 
* Dialogue 
* Autocompletion
* Machine translation
* Fluency evaluation

Today, LMs are commonly used to generate pretrained representations of text that encode some notion of language understanding for downstream NLP tasks. But can a language model be used as a knowledge base? 

<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/227144882-888d7ae0-b293-4af3-a365-5a828c410c0f.PNG" width="550" title="Transformers">
</p>

Predictions made by LMs are generally make sense (e.g. the correct types), but are not all factually correct. The cause of this are as follows:

* Unseen facts: Some facts may not have occurred in the training corpora at all
* Rare facts: LM hasn’t seen enough examples during training to memorize the fact
* Model sensitivity: LM may have seen the fact during training, but is sensitive to the phrasing of the prompt.Correctly answers “x was made in y” templates but not “x was created in y”

<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/227145742-ac074bf9-5a5e-4bf6-8b6f-05ae5d0270b8.PNG" width="550" title="Transformers">
</p>

<h3> Querying language models as knowledge bases </h3>

Querying language models as knowledge bases is a recent development in natural language processing (NLP) that involves using large-scale language models like GPT-3 and BERT as a source of knowledge about the world. This approach is based on the idea that language models have been trained on massive amounts of text data, and have learned to represent the relationships between words and concepts in a way that reflects the real-world knowledge they contain.

One way to query a language model as a knowledge base is to input a natural language question or statement and extract relevant information from the model's output. For example, a user could ask a language model like GPT-3 "Who is the current president of France?" and the model could provide a response such as "The current president of France is Emmanuel Macron."

Another approach is to use a language model to generate a text summary or answer based on a given input text. For example, a user could input a news article about a recent event, and the language model could generate a summary or answer to a specific question based on the content of the article.

Querying language models as knowledge bases has many potential applications in fields such as information retrieval, question answering, and conversational agents. However, there are also challenges and limitations to this approach, including the potential for errors and biases in the model's output, and the need for effective methods to validate and verify the information provided by the model.

<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/227146059-c85fb2f6-54f2-4370-8b3e-a53e4fe850d0.PNG" width="550" title="Transformers">
</p>

<h3>Techniques to add knowledge to LMs </h3>

<h4>Pretrained entity embeddings </h4>
Pretrained entity embeddings is a technique for adding external knowledge to a language model by incorporating pre-trained embeddings for named entities, such as people, organizations, and locations, into the model's internal representations. Named entity recognition (NER) is a common pre-processing step for many natural language processing (NLP) tasks, and entity embeddings can help improve the performance of these models by adding additional context and information about the entities mentioned in the text.

To use pretrained entity embeddings, a language model is first trained on a large corpus of text data, as is typical in NLP. Then, external knowledge sources are added by incorporating pretrained embeddings for entities such as people, organizations, and locations, which have been trained on a separate corpus of text data. These embeddings can be added to the model as additional input features, or they can be used to initialize the model's internal embeddings.

The benefits of using pretrained entity embeddings include improved accuracy and robustness on tasks such as named entity recognition and relation extraction, as well as the ability to incorporate external knowledge into the model without requiring additional training data. This can be particularly useful in domains where training data is limited, such as in the medical or legal domains.

However, there are also challenges to using pretrained entity embeddings, including the potential for biases and inaccuracies in the external knowledge sources, and the need for effective methods to integrate this knowledge into the model's internal representations. 

<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/227146813-fff2a802-cdc9-4164-95a0-d22f2f321686.PNG" width="550" title="Transformers">
</p>

<h4> ERNIE(Enhanced Language Representation with Informative Entities)</h4>

ERNIE is a large-scale language model developed by Baidu's Institute of Deep Learning (IDL) that is designed to better capture the relationship between words and entities in natural language text. ERNIE is based on the popular transformer architecture used in models like BERT and GPT, but incorporates additional training objectives that focus on entity-level tasks, such as entity recognition and relation extraction.

One of the key innovations of ERNIE is its use of entity-level masking during training, which involves masking out entire named entities in the input text and training the model to predict them based on the surrounding context. This allows the model to better capture the relationships between words and entities, and has been shown to improve performance on tasks such as named entity recognition and entity linking. ERNIE also incorporates additional training objectives that focus on semantic and syntactic relationships between entities, such as entity classification and entity relation extraction. These objectives are designed to help the model better understand the complex relationships between entities in natural language text, and have been shown to improve performance on a wide range of NLP tasks.



