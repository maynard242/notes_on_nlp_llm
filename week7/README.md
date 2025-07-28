# Week 7: Prompting, Sampling, and In-Context Learning

This week focuses on the practical aspects of interacting with and controlling the output of a trained LLM. We move from training models to using them effectively.

### 7.1 Controlling Generation: Sampling Strategies
An LLM outputs a probability distribution over the vocabulary. How we select the next token from this distribution has a major impact on the generated text.
* **Greedy Decoding**: Always picking the most likely token. Deterministic but can be repetitive.
* **Sampling with Temperature**: Controls the randomness of the output. Higher temperature increases diversity, lower temperature makes it more deterministic.
* **Top-k and Top-p (Nucleus) Sampling**: Methods to truncate the probability distribution to avoid sampling from the long tail of unlikely tokens, improving coherence.

### 7.2 Prompt Engineering
The art and science of designing effective prompts to elicit desired behaviors from an LLM without updating its weights.
* **Elements of a Good Prompt**: Role, task, situation, format, constraints, and examples.
* **In-Context Learning (Few-Shot Prompting)**: Providing a few examples of the task within the prompt itself, which the model uses as a pattern to follow for the actual query.

### 7.3 Hallucinations and Mitigation
A fundamental challenge where LLMs generate plausible but factually incorrect or nonsensical information.
* **Causes**: A result of the model's objective to generate probable sequences, not true statements, combined with gaps or inaccuracies in its training data.
* **Mitigation with Retrieval-Augmented Generation (RAG)**: Grounding the model's response in factual information. A retriever first fetches relevant documents from a trusted knowledge base, and these documents are then provided to the LLM as context in the prompt, instructing it to base its answer on the provided text.

### Key Resources for Week 7
* **Primary Text**: *The Hundred-Page Language Models Book*, Chapter 5, Sections 5.4, 5.7, 5.8.
* **Key Paper**: *Language Models are Few-Shot Learners* (Brown et al., 2020 - GPT-3).
* **Practical Guide**: OpenAI's Prompt Engineering Guide.