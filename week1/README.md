# Week 1: Machine Learning & NLP Fundamentals

This foundational week unifies the essential prerequisites for modern NLP. We will cover the core mathematical machinery of machine learning and the fundamental linguistic concepts that motivate text processing techniques.

### 1.1 Machine Learning First Principles
Before tackling language, we must understand how models learn. This section covers the mathematical engine of deep learning.
* **Core Concepts**: Models, parameters, and the four-step learning process (data collection, model definition, loss function, optimization).
* **Mathematical Toolkit**: Vectors, matrices, and their operations as the language of data representation.
* **The Learning Algorithm**: A deep dive into **Gradient Descent** as the universal optimization algorithm for neural networks.
* **Implementation**: Understanding **Automatic Differentiation** (Autograd) as the practical tool that makes training complex models feasible.

### 1.2 The Text Pre-processing Cascade
This section covers the pipeline for converting raw, unstructured text into a format suitable for machine learning, with a focus on the trade-offs involved.
* **Normalization**: Lowercasing, punctuation removal, and their impact on information content.
* **Tokenization**: The evolution from word/sentence tokenization to modern **Subword Tokenization** (BPE, WordPiece) to handle large vocabularies and out-of-vocabulary words.
* **Morphological Normalization**: The distinction between crude, rule-based **Stemming** and principled, dictionary-based **Lemmatization**.

### Key Resources for Week 1
* **Primary Text**: *The Hundred-Page Language Models Book*, Chapter 1: "Machine Learning Basics".
* **Primary Lecture**: Stanford CS224N Winter 2021 | Lecture 1 - Intro and Word Vectors (https://www.youtube.com/watch?v=DzpHeXVSC5I).
* **Key Paper**: *A Neural Probabilistic Language Model* (Bengio et al., 2003) - The paper that introduced the idea of learning a distributed representation for words.