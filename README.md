# 🤖 Fine-Tuned Phi-4 Model with RAG (FAISS + Unsloth)

This repository contains a fine-tuned version of the [Phi-4](https://huggingface.co/unsloth/phi-4) language model using a question-answering dataset. The project integrates **Retrieval-Augmented Generation (RAG)** with **FAISS** for document retrieval and **Unsloth** for efficient model fine-tuning and inference.

---

## 📌 Overview

- 🧠 Base model: [Unsloth's Phi-4](https://huggingface.co/unsloth/phi-4)  
- 🔧 Fine-tuned on private question–answer pairs derived from document content  
- 🔍 Retrieval-Augmented Generation using **FAISS** for semantic similarity  
- ⚡ Performance-optimized with **Unsloth** (LoRA + memory-efficient inference)  
- ✅ Manually evaluated responses after fine-tuning and after RAG integration

---

## 📁 Dataset Format (Private)

While the dataset is private, you can recreate a similar one easily. The format is based on creating **question–answer** pairs from a single document. For example:

```json
{
  "question": "What are the main causes of climate change?",
  "answer": "The main causes include greenhouse gas emissions from human activities such as burning fossil fuels and deforestation."
}
```

Steps to create your dataset:

1. Select any document (e.g., academic paper, article, book chapter).
2. Extract or manually write relevant questions and answers.
3. Format as JSON or CSV with `question` and `answer` fields.

---

## 🛠️ Installation

Install the necessary libraries:

```bash
pip install transformers unsloth faiss-cpu
```

> If you're using a GPU, install `faiss-gpu` instead of `faiss-cpu`.

---

## 🔧 To Do

- [ ] Add LangChain support  
- [ ] Implement automatic evaluation script  
- [ ] Add a web UI with Gradio or Streamlit  


