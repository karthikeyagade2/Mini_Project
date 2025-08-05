# Text Analysis Tool: AI-Generated & Plagiarism Detection with RoBERTa

![Python](https://img.shields.io/badge/Python-3.9+-blue)
![HuggingFace](https://img.shields.io/badge/Transformers-RoBERTa-purple)
![Gradio](https://img.shields.io/badge/UI-Gradio-green)
![License](https://img.shields.io/badge/license-MIT-green)
![NLP](https://img.shields.io/badge/Type-NLP-yellow)

> An NLP-powered system leveraging RoBERTa to detect **AI-generated content** and **plagiarism** in text, enhancing academic integrity and content authenticity.

---

## Project Overview

**Text Analysis Tool** is a RoBERTa-based application designed to distinguish between:
- **Human-written text**
- **AI-generated text**
- **Plagiarized content**

This tool is intended for educational institutions, publishers, researchers, and content creators seeking to verify originality and detect unethical content generation or duplication.

---

## Key Features

- Detects AI-generated content using RoBERTa fine-tuned on diverse datasets
- Plagiarism detection using cosine similarity-based comparison
- Provides both *Human Score* and *Plagiarism Score*
- Built-in Gradio UI for easy testing and deployment
- Handles diverse text inputs, including long-form content
- Outputs real-time classification and similarity scores

---

## Project Structure

```text
Text-Analysis-Tool/
├── data/              # Input datasets (human + AI-generated)
├── models/            # Fine-tuned RoBERTa model
├── ui/                # Gradio-based UI scripts
├── utils/             # Tokenizers, scorers, preprocessing helpers
├── notebooks/         # Jupyter notebooks for training & evaluation
├── results/           # Accuracy, F1-score, confusion matrix, logs
├── requirements.txt   # Dependency list
└── README.md          # Project documentation
```
## Model Details
Model: RoBERTa-base (from HuggingFace Transformers)

Tokenization: Byte Pair Encoding (BPE)

Fine-tuned on:

AI-generated samples (GPT-4, LLaMA, Claude, Gemini, Falcon)

Human-written samples (from Kaggle & academic corpora)

Evaluation:

Accuracy: ~91%

F1 Score: ~89%

Real-time classification (<2s)
## UI Demo
Using Gradio, users can:

Paste or upload any text

View:

Human Score (%)

Plagiarism Score (%)

Detect and analyze content instantly

(Optional) Future versions may integrate with LMS or CMS systems




