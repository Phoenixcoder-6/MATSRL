# 🧠 MATSRL: Multi-Agent Text Summarization using Reinforcement Learning

**MATSRL** (Multi-Agent Text Summarization using Reinforcement Learning) is a novel framework that decomposes the abstractive summarization task into specialized subtasks, handled by dedicated agents. By combining the strengths of **BERT**, **T5**, **BART**, and **Reinforcement Learning (A2C)**, MATSRL produces high-quality, coherent, and human-readable summaries from long-form text documents.

---

## 📌 Overview

Traditional abstractive summarization models attempt to perform sentence selection, rewriting, and summary generation in a single step, often leading to poor control and interpretability. **MATSRL** introduces a modular approach with **three intelligent agents**:

- **Extractor Agent (BERT + A2C)**: Learns to select key sentences from the input using Advantage Actor-Critic (A2C) reinforcement learning.
- **Simplifier Agent (T5)**: Rewrites extracted sentences into simpler, more concise representations.
- **Synthesizer Agent (BART)**: Merges simplified content and generates the final abstract summary.

Each agent operates independently yet collaboratively to improve summary quality, reduce redundancy, and enhance readability.

---

## ⚙️ Architecture
![Screenshot 2025-05-16 012141](https://github.com/user-attachments/assets/92d7af3f-520e-401d-81c9-8e0b7445b5b9)

