<div align="center">

# 🧠 LLM From Scratch

**Building and Fine-Tuning a GPT-style Language Model from the Ground Up**

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)](https://pytorch.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)

*A hands-on project implementing a GPT-2 style transformer language model from scratch using PyTorch, followed by instruction fine-tuning on real-world datasets.*

---

</div>

## 📖 Overview

This repository contains two core notebooks that walk through the full lifecycle of building a Large Language Model:

| Notebook | Description |
|----------|-------------|
| `01_gpt_from_scratch.ipynb` | Build a GPT-2 (124M) architecture from scratch — multi-head attention, transformer blocks, text generation |
| `02_instruction_finetuning.ipynb` | Fine-tune the model on the [AG News](https://huggingface.co/datasets/fancyzhx/ag_news) classification dataset using instruction-tuning techniques |

## 🏗️ Project Structure

```
LLM-From-Scratch/
├── 📓 01_gpt_from_scratch.ipynb      # Full GPT implementation from scratch
├── 📓 02_instruction_finetuning.ipynb # Instruction fine-tuning pipeline
├── 📂 data/
│   └── pride_and_prejudice.txt        # Training corpus (Project Gutenberg)
├── 📄 requirements.txt               # Python dependencies
├── 📄 LICENSE                         # MIT License
├── 📄 .gitignore                      # Git ignore rules
└── 📄 README.md                       # You are here!
```

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- CUDA-compatible GPU (recommended) or CPU

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Rishi210904/Project-1-of-LLM.git
   cd Project-1-of-LLM
   ```

2. **Create a virtual environment** (optional but recommended)
   ```bash
   python -m venv venv
   source venv/bin/activate   # Linux/Mac
   venv\Scripts\activate      # Windows
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter**
   ```bash
   jupyter notebook
   ```

## 📓 Notebooks

### 1. GPT From Scratch (`01_gpt_from_scratch.ipynb`)

Implements the complete GPT-2 (124M) architecture from the ground up:

- **Tokenization** — BPE tokenization using OpenAI's `tiktoken`
- **Embedding Layers** — Token + positional embeddings
- **Multi-Head Self-Attention** — Causal (masked) attention mechanism
- **Transformer Block** — Layer normalization, feed-forward network, residual connections
- **GPT Model** — Full model assembly with configurable hyperparameters
- **Text Generation** — Autoregressive next-token prediction

**Training Data:** *Pride and Prejudice* by Jane Austen (Project Gutenberg)

### 2. Instruction Fine-Tuning (`02_instruction_finetuning.ipynb`)

Demonstrates how to fine-tune the pre-trained model for downstream tasks:

- **Dataset** — AG News (news article classification)
- **Technique** — Instruction-style fine-tuning
- **Libraries** — Hugging Face `datasets`, `safetensors` for weight loading
- **Evaluation** — Performance metrics on the classification task

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| [PyTorch](https://pytorch.org/) | Deep learning framework |
| [tiktoken](https://github.com/openai/tiktoken) | BPE tokenizer (GPT-2 compatible) |
| [matplotlib](https://matplotlib.org/) | Training loss visualization |
| [Hugging Face Datasets](https://huggingface.co/docs/datasets/) | AG News dataset loading |
| [safetensors](https://github.com/huggingface/safetensors) | Safe model weight serialization |
| [tqdm](https://tqdm.github.io/) | Progress bars |

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Andrej Karpathy](https://karpathy.ai/) for inspiring the "build from scratch" approach
- [Sebastian Raschka](https://sebastianraschka.com/) and the [LLMs from Scratch](https://github.com/rasbt/LLMs-from-scratch) project
- [Project Gutenberg](https://www.gutenberg.org/) for the training corpus
- [Hugging Face](https://huggingface.co/) for datasets and tools

---

<div align="center">

**⭐ Star this repo if you found it helpful!**

</div>
