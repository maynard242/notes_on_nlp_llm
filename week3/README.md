# Week 3: Sequential Processing with Recurrent Neural Networks (RNNs)

Before the Transformer, Recurrent Neural Networks were the state-of-the-art for sequence modeling. Understanding their architecture and, more importantly, their limitations is crucial for appreciating why the Transformer was such a revolutionary development.

### 3.1 The Architecture of Recurrence
RNNs process sequences token-by-token, maintaining a "memory" or "hidden state" that captures information from previous steps.
* **The Elman RNN**: The simplest form of RNN, where the hidden state at time `t` is a function of the input at time `t` and the hidden state at time `t-1`.
* **The Vanishing Gradient Problem**: The core challenge in training RNNs. As information propagates through long sequences, gradients can shrink exponentially, making it difficult for the model to learn long-range dependencies.
* **Long Short-Term Memory (LSTM)**: A more complex RNN variant with a gating mechanism (input, forget, and output gates) designed specifically to mitigate the vanishing gradient problem and better regulate information flow.

### 3.2 RNNs as Language Models
* **Training**: How an RNN is trained for causal language modeling by processing a sequence and using the hidden state at each step to predict the next token.
* **Limitations**:
    1.  **Sequential Bottleneck**: The inability to parallelize computations within a sequence, making them slow to train on modern hardware.
    2.  **Long-Range Dependencies**: Despite LSTMs, capturing very long-range context remains challenging.

### Key Resources for Week 3
* **Primary Text**: *The Hundred-Page Language Models Book*, Chapter 3: "Recurrent Neural Network".
* **Key Paper**: *Long Short-Term Memory* (Hochreiter & Schmidhuber, 1997).
* **Visual Guide**: *Understanding LSTMs* by Chris Olah (http://colah.github.io/posts/2015-08-Understanding-LSTMs/).