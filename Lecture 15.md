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


<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/227146059-c85fb2f6-54f2-4370-8b3e-a53e4fe850d0.PNG" width="550" title="Transformers">
</p>


