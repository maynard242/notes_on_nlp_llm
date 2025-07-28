# Week 2: Classical Language Modeling & Representations

This week traces the evolution of text representation, from sparse, count-based methods to the revolutionary concept of dense word embeddings. We also introduce the formal task of language modeling and methods for its evaluation.

### 2.1 Sparse Representations
The earliest methods represented documents as high-dimensional, sparse vectors based on word counts.
* **Bag-of-Words (BoW)**: Represents a document as a vector of word counts, ignoring grammar and word order.
* **TF-IDF (Term Frequency-Inverse Document Frequency)**: Refines BoW by weighting words based on their importance in a document relative to the corpus.

### 2.2 Dense Embeddings: Word2Vec and GloVe
A major breakthrough that represents words as dense, low-dimensional vectors, capturing semantic relationships.
* **Word2Vec (Predictive Method)**: Learns embeddings by predicting a word from its context (**CBOW**) or predicting context from a word (**Skip-Gram**).
* **GloVe (Count-based Method)**: Learns embeddings from a global word-word co-occurrence matrix, arguing that the *ratio* of co-occurrence probabilities encodes meaning.

### 2.3 Language Modeling and Evaluation
* **The Task**: Formally defining a language model as a system that computes the probability of the next token given a context.
* **Evaluation Metrics**:
    * **Perplexity**: A standard intrinsic measure of how well a probability model predicts a sample. Lower perplexity indicates a better model.
    * **ROUGE**: An extrinsic metric used for tasks like summarization, measuring n-gram overlap between generated and reference texts.
    * **Human Evaluation**: The gold standard, using Likert scales or pairwise comparisons (Elo rating) to assess qualities like fluency and coherence.

### Key Resources for Week 2
* **Primary Text**: *The Hundred-Page Language Models Book*, Chapter 2: "Language Modeling Basics".
* **Primary Papers**:
    * *Efficient Estimation of Word Representations in Vector Space* (Mikolov et al., 2013 - Word2Vec).
    * *GloVe: Global Vectors for Word Representation* (Pennington et al., 2014).
* **Visual Guide**: *The Illustrated Word2Vec* by Jay Alammar.