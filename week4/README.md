# Week 4: The Transformer Architecture

This week is a deep, mechanical dive into the Transformer architecture. We will deconstruct its components to understand how it overcomes the limitations of RNNs by relying entirely on self-attention, enabling massive parallelization and superior handling of long-range dependencies.

### 4.1 Self-Attention: The Core Mechanism
The innovation that allows the model to weigh the importance of all other words in the sequence when processing a given word.
* **Queries, Keys, and Values (QKV)**: The core abstraction for calculating attention scores.
* **Scaled Dot-Product Attention**: The mathematical formulation `Attention(Q,K,V) = softmax(QK^T/√d_k)V`.

### 4.2 Architectural Components
* **Multi-Head Attention**: Performing self-attention multiple times in parallel to allow the model to focus on different types of information from different representation subspaces.
* **Positional Encodings**: Injecting information about word order. We will contrast the original sinusoidal encodings with modern **Rotary Position Embeddings (RoPE)**, which apply position-dependent rotations to Q and K vectors.
* **The Transformer Block**: Assembling the components: residual connections, **RMSNorm** (a modern, efficient alternative to LayerNorm), and position-wise feed-forward networks.

### 4.3 Inference Optimization
* **Key-Value (KV) Caching**: A crucial optimization for efficient autoregressive generation, where the Key and Value vectors for previous tokens are cached to avoid redundant computation.

### Key Resources for Week 4
* **Primary Text**: *The Hundred-Page Language Models Book*, Chapter 4: "Transformer".
* **Primary Paper**: *Attention Is All You Need* (Vaswani et al., 2017).
* **Primary Visual Guide**: *The Illustrated Transformer* by Jay Alammar.
* **Primary Lecture**: Stanford CS224N | 2023 | Lecture 8 - Self-Attention and Transformers.