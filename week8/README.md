# Week 8: Alignment and Advanced Topics

The final week covers the critical process of aligning LLMs with human values to make them helpful and harmless, and provides a survey of cutting-edge topics that define the current research frontier.

### 8.1 Alignment with Human Preferences
Techniques to refine a model's behavior beyond simply following instructions, steering it towards qualities like helpfulness, honesty, and harmlessness.
* **Reinforcement Learning from Human Feedback (RLHF)**: The classic three-step process: (1) Supervised fine-tuning, (2) training a reward model on human preference data, and (3) fine-tuning the SFT model using RL (PPO) to maximize the reward.
* **Direct Preference Optimization (DPO)**: A more direct and stable alternative that achieves the goal of RLHF with a simpler classification loss, eliminating the need for a separate reward model and the complexities of RL.

### 8.2 Survey of Advanced Topics
A look at current research areas extending the capabilities of LLMs.
* **Mixture of Experts (MoE)**: An architectural pattern to increase model capacity efficiently by sparsely activating "expert" sub-networks.
* **Model Merging**: Techniques for combining multiple pre-trained models to leverage their complementary strengths.
* **Model Compression**: Methods like quantization and pruning to reduce the size and computational cost of LLMs for deployment.
* **Advanced Reasoning**: Techniques like Chain-of-Thought (CoT) and Tree-of-Thought (ToT) that prompt the model to generate intermediate reasoning steps to solve complex problems.
* **Vision Language Models (VLMs)**: Integrating vision encoders with LLMs to process and reason about both text and images.
* **Language Model Security**: Understanding vulnerabilities like prompt injection and jailbreaking.

### Key Resources for Week 8
* **Primary Text**: *The Hundred-Page Language Models Book*, Chapter 6: "Further Reading".
* **Primary Papers**:
    * *Training language models to follow instructions with human feedback* (Ouyang et al., 2022 - InstructGPT/RLHF).
    * *Direct Preference Optimization: Your Language Model is Secretly a Reward Model* (Rafailov et al., 2023 - DPO).
* **Technical Blog**: *Hugging Face Blog on RLHF*.