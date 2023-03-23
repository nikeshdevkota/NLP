# Natural Language Processing
## Lesson 12

<h3> Natural Language Generation</h3>

Natural language generation (NLG) is a subfield of artificial intelligence (AI) that involves the automatic generation of natural language text by a computer or machine. 
NLG systems use algorithms and rules to transform data, structured input, or other forms of non-linguistic information into natural language text.

<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/227134868-e1c0fae2-319e-4168-8493-17fc4698b20f.PNG" width="550" title="Transformers">
</p>

NLG is a multi-disciplinary field that draws on expertise from computer science, computational linguistics, psychology, and linguistics. It is used in a wide range of applications, including chatbots, virtual assistants, automated news reports, product descriptions, and personalized recommendations.
There are several approaches to NLG, including rule-based systems, template-based systems, and machine learning-based systems. Rule-based systems use a set of predefined rules to generate natural language text. Template-based systems use pre-written templates to generate text that can be customized based on the input data. Machine learning-based systems use statistical models and deep learning algorithms to generate natural language text based on large amounts of training data.
NLG can be used to generate text in a variety of styles, including informative, persuasive, and entertaining. It can also be used to generate text in multiple languages, making it a powerful tool for global communication.

<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/227135180-f9368632-48e9-4ac1-ac9b-60fb31d5fe35.PNG" width="550" title="Transformers">
</p>

<h3> Decoding: Top-k sampling </h3>

Top-k sampling is a decoding strategy used in natural language processing (NLP) to generate text from a language model. It involves selecting the top k words with the highest probabilities from the model's output distribution at each step of the decoding process, and sampling from this subset of words to generate the next word in the sequence.For example, if k=5, the model's output distribution might be [0.3, 0.2, 0.1, 0.1, 0.1, 0.1, 0.05, 0.05, 0.05, 0.05] for a given time step. Top-k sampling would involve selecting the top 5 words with the highest probabilities (in this case, the first 5 words), and sampling from this subset to generate the next word in the sequence.

<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/227136427-0faf42d3-3751-4c19-a3e0-aa007b80c67a.PNG" width="550" title="Transformers">
</p>

Top-k sampling is useful for avoiding the problem of repetition in language generation, where the model tends to generate the same words or phrases over and over again. By constraining the choices for the next word to a smaller set of the most likely options, top-k sampling can encourage the model to generate more diverse and interesting text. One limitation of top-k sampling is that it can lead to abrupt changes in the tone or style of the generated text, as the model may switch between different words or phrases based solely on their probability of occurrence. This can be mitigated by adjusting the value of k or using other decoding strategies, such as beam search or nucleus sampling.

<p align="center">
<img src= "https://user-images.githubusercontent.com/45029614/227136674-90b5b81d-f2bf-4056-80f9-5d7df3916fd5.PNG" width="550" title="Transformers">
</p>

<h3> Decoding: Top-p (nucleus) sampling </h3>

Top-p, also known as nucleus sampling, is a decoding strategy used in natural language processing (NLP) to generate text from a language model. It involves selecting the smallest possible set of words that make up a cumulative probability of p, and sampling from this set of words to generate the next word in the sequence.

For example, if p=0.9, the model's output distribution might be [0.05, 0.02, 0.01, 0.1, 0.05, 0.1, 0.01, 0.02, 0.2, 0.44] for a given time step. Nucleus sampling would involve selecting the smallest set of words that make up at least 90% of the total probability mass (in this case, the first 9 words), and sampling from this subset to generate the next word in the sequence.

Nucleus sampling is useful for generating diverse and interesting text, while still maintaining some level of coherence and relevance to the context. It allows the model to explore a wider range of possible words and phrases, while still ensuring that the generated text is likely to be related to the input text.

One advantage of nucleus sampling over top-k sampling is that it avoids the problem of abrupt changes in the tone or style of the generated text, as it maintains a more gradual transition between words and phrases. However, nucleus sampling can be computationally expensive, as it requires the model to compute the cumulative probabilities of all possible words at each time step.

