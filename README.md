# 🤖 GPT Series Deep Learning Models Explanation

## 🎯 Introduction

This repository aims to provide a comprehensive and intuitive explanation of the deep learning model architecture underlying OpenAI's GPT series of language models, including GPT-4, GPT-3, GPT-2, and the original GPT. Based on the Transformer model, these architectures are complex, and understanding them can be quite challenging. Here, we break down the process into its constituent parts using a sentence example "The dog bit the man".

## 🚀 GPT Series and Transformer Architecture

The GPT series of models, including GPT-4, GPT-3, GPT-2, and the original GPT, are based on the Transformer architecture and follow a similar design philosophy. The main differences among these models lie in the scale (number of model parameters) and training data. Let's take a closer look at the steps involved in the Transformer architecture.

### 🧩 Transformer Architecture: A Closer Look

The Transformer architecture is the backbone of the GPT models and represents a significant breakthrough in Natural Language Processing. It addresses the limitations of sequential processing in recurrent neural networks by enabling parallelization and capturing dependencies regardless of their distance in the input sequence. Here, we dive into the steps involved in this innovative architecture:

1. **Embedding Layer**: the initial step in the Transformer architecture is the transformation of each word into a unique vector representation. This allows the model to process the input text numerically:
    - "The" --> [⚫]
    - "dog" --> [🐶]
    - "bit" --> [🦷]
    - "the" --> [⚫]
    - "man" --> [👨]

2. **Positional Encoding**: to preserve the sequence information intrinsic to language, position information is added to each word vector:
    - "The (1)" --> [⚫1️⃣]
    - "dog (2)" --> [🐶2️⃣]
    - "bit (3)" --> [🦷3️⃣]
    - "the (4)" --> [⚫4️⃣]
    - "man (5)" --> [👨5️⃣]

3. **Multi-Head Attention**: this step involves determining the dependencies between each word and the others in the sentence. The connections (—) between words represent these dependencies, with the thickness of the connection indicating the degree of dependency:
    - "The (1)" —— "dog (2)" ——— "bit (3)" —— "the (4)" —— "man (5)"

4. **Feedforward Network**: the feedforward network can be visualized as a funnel (🔽) that processes and refines the information from each word:
    - "The (1)" ——🔽—— "dog (2)" ——🔽—— "bit (3)" ——🔽—— "the (4)" ——🔽—— "man (5)"

5. **Layer Normalization and Residual Connection**: balancing the information from each word is achieved through mechanisms similar to sliders (🔲🔳):
    - "The (1)" ——🚫🔲🔳—— "dog (2)" ——🔽🔲🔳—— "bit (3)" ——🔽🔲🔳—— "the (4)" ——🔽🔲🔳—— "man (5)"

6. **Output Layer**: the culmination of the process is the output layer, where the model predicts the next word in the sentence based on the learned information. For example, given the sentence "The dog bit the man," the model might suggest the word "injured" (🩹):
    - "The dog bit the man" ——> "injured (🩹)"

This detailed examination of the Transformer architecture sheds light on the intricate processes that empower the GPT series to generate contextually relevant and creative text.

## 📊 GPT Model Parameters

One of the significant differences between each GPT model is the number of parameters:

- 🎈 GPT (Original): 117M parameters
- 🎈🎈 GPT-2: 1.5B parameters
- 🎈🎈🎈 GPT-3: 175B parameters
- 🎈🎈🎈🎈 GPT-4: 100T (trillion) parameters

These models' increasing complexity correlates with their ability to understand and generate increasingly nuanced text.

## 📚 Why this Repository?

Understanding the Transformer architecture and deep learning models like the GPT series can be a complex process. This repository's goal is to distill these complexities into more comprehensible units, thereby allowing enthusiasts, students, and even seasoned developers to get a clear understanding of how these models function.

## 📖 Further Reading

We encourage interested readers to delve deeper into the fascinating world of language models. To that end, here are a few resources:

- [Attention is All You Need](https://arxiv.org/abs/1706.03762) - The original Transformer paper by Vaswani et al.
- [The Illustrated Transformer](http://jalammar.github.io/illustrated-transformer/) - A highly recommended blog post with clear explanations and helpful diagrams.
- [OpenAI's GPT-2 Paper](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf) - This paper provides further insights into the use of Transformer architecture in language models.

Thank you for visiting this repository! Feel free to contribute and expand on this basic explanation.
