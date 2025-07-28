# Week 5: The Rise of Large Language Models (LLMs)

This week explores how the Transformer architecture was scaled up to create the massive models we know today. We will cover the dominant pre-training paradigms and the empirical laws that guide large-scale training.

### 5.1 The Pre-train, Fine-tune Paradigm
The two-stage process that defines modern NLP:
1.  **Pre-training**: Training a large model on a massive, unlabeled corpus using a self-supervised objective.
2.  **Fine-tuning**: Adapting the general-purpose model to a specific task using a smaller, labeled dataset.

### 5.2 Foundational LLM Architectures
* **BERT (Encoder-Only)**: Pre-trained with **Masked Language Modeling (MLM)** for deep bidirectional understanding. Ideal for NLU tasks.
* **GPT (Decoder-Only)**: Pre-trained with **Causal Language Modeling (CLM)** for autoregressive text generation. The foundation of modern generative AI.
* **T5 (Encoder-Decoder)**: Pre-trained with a **span corruption** objective under a unified "text-to-text" framework, making it versatile for sequence-to-sequence tasks.

### 5.3 Scaling Laws and Data Curation
* **Scaling Laws**: The empirical finding that model performance scales predictably with model size, dataset size, and compute. The **Chinchilla** paper revised these laws, emphasizing the critical importance of dataset size.
* **Dataset Curation**: The massive data engineering effort behind LLMs, including collection, cleaning, filtering, deduplication, and decontamination.

### Key Resources for Week 5
* **Primary Text**: *The Hundred-Page Language Models Book*, Chapter 5: "Large Language Model".
* **Primary Papers**:
    * *BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding* (Devlin et al., 2018).
    * *Training Compute-Optimal Large Language Models* (Hoffmann et al., 2022 - Chinchilla).
* **Primary Lecture**: Stanford CS224N | 2023 | Lecture 9 - Pre-training and Transfer Learning.