# Week 6: Fine-Tuning and Adaptation

A pre-trained model possesses general knowledge, but fine-tuning is required to specialize it for specific tasks. This week focuses on modern, efficient techniques for model adaptation.

### 6.1 Supervised Fine-Tuning (SFT)
The process of adapting a model to a specific task by training it on a labeled dataset. This is the foundational step for both task-specific models and for preparing a model for alignment.

### 6.2 The Challenge of Full Fine-Tuning
Updating all parameters of a multi-billion parameter model is computationally expensive and memory-intensive, creating a need for more efficient methods.

### 6.3 Parameter-Efficient Fine-Tuning (PEFT)
A family of techniques that freezes the vast majority of the base model's parameters and trains only a small number of new or existing parameters.
* **Low-Rank Adaptation (LoRA)**: The most popular PEFT method. It injects small, trainable low-rank matrices into the Transformer layers. Instead of updating the large weight matrix `W`, LoRA learns a low-rank update `W + BA`, where only `B` and `A` are trained.
* **QLoRA (Quantized LoRA)**: An even more efficient version of LoRA that fine-tunes an adapter on top of a base model that has been quantized to a lower precision (e.g., 4-bit).

### 6.4 LLMs as Classifiers
Exploring how to adapt a generative LLM for classification tasks, either by training it to generate the class label as text or by adding a classification head on top of the final layer's embeddings.

### Key Resources for Week 6
* **Primary Text**: *The Hundred-Page Language Models Book*, Chapter 5, Sections 5.2, 5.3, 5.5, 5.6.
* **Primary Paper**: *LoRA: Low-Rank Adaptation of Large Language Models* (Hu et al., 2021).
* **Technical Blog**: *Hugging Face PEFT Library Documentation*.