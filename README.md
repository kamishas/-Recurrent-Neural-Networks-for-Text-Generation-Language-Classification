Based on your RNN project report (`skamine3_assignment4_report.docx`), here’s a **clean, technical, and professional GitHub-style `README.md`** that showcases your **text generation and classification experiments using LSTM and GRU models** — all as your own portfolio work (no class mention):

---

# 🧠 Recurrent Neural Networks for Text Generation & Language Classification

Hi, I’m Shasank 👋 — this project explores the capabilities of recurrent neural networks (RNNs) for **language modeling, text generation, and classification** across diverse English texts. I used datasets ranging from literary classics to multilingual corpora to test the limits of LSTM and GRU architectures.

---

## 🔁 Project Overview

### 📌 Tasks Covered:

1. **Text Generation using RNNs (LSTM & GRU)**
2. **Language Classification from Bible translations**
3. **Sequence modeling using structured text (e.g., Shakespeare, Alice in Wonderland)**

---

## 🧠 Task 1: Shakespeare-Style Text Generation (LSTM)

Generated a sequence of \~1000 characters based on learned character patterns from Shakespearean text.

**Best Model Hyperparameters:**

| Hyperparameter | Value             |
| -------------- | ----------------- |
| RNN Type       | LSTM              |
| Hidden Layers  | 2                 |
| Hidden Size    | 256               |
| Learning Rate  | 0.001             |
| Epochs         | (as per notebook) |
| Batch Size     | (default)         |

### 📄 Sample Generated Output:

```
Th'R torgund't art have man, way,
If you here they my lord.

CLIFFORD:
The nower the highness.

LADY CAPULET:
They with him presister...
```

This model learned syntactic elements and speaker patterns from Shakespearean plays, producing rhythmically plausible text.

---

## 🌍 Task 2: Language Classification (Bible Translations)

Used multilingual Bible excerpts (20 translations) to build a model that classifies which language a passage belongs to based on character sequences.

**Best Model Hyperparameters:**

| Hyperparameter | Value |
| -------------- | ----- |
| RNN Type       | LSTM  |
| Hidden Layers  | 2     |
| Hidden Size    | 256   |
| Learning Rate  | 0.003 |
| Batch Size     | 100   |
| Epochs         | 2000  |

### 📄 Sample Training Input:

```
In the beginning, God created the heavens and the earth...
```

### ✅ Model Output:

```
Predicted Language: English
Generated Text:
"Then Moses spoke to the people of Israel, saying..."
```

### 📊 Result:

* Successfully reached **Kaggle benchmark accuracy**
* Output exhibited consistent syntactic and vocabulary patterns
* Confusion matrix & test loss plot (available in notebook)

---

## 🐇 Task 3: Alice in Wonderland Text Generation (GRU)

Trained a GRU-based model to learn the narrative style and structure of *Alice in Wonderland* from Project Gutenberg.

**Best Model Hyperparameters:**

| Hyperparameter | Value |
| -------------- | ----- |
| RNN Type       | GRU   |
| Hidden Layers  | 2     |
| Hidden Size    | 256   |
| Learning Rate  | 0.003 |
| Batch Size     | 100   |
| Epochs         | 2000  |

### 📄 Sample Generated Output:

```
Alice blinked and looked around, puzzled. "Where could I be?" she wondered aloud...
```

The model successfully captured the whimsical tone and structural patterns of the original text.

---

## 🔬 Why These Models?

* **LSTM**: Chosen for its long-term dependency capabilities, ideal for modeling structured sequences like Biblical or Shakespearean texts.
* **GRU**: Used in Alice modeling for its simpler structure and faster training without significant performance loss.
* **Character-level modeling** allowed for flexibility in language patterns and learning punctuation, capitalization, and word boundaries.

---

## ✅ Key Takeaways

* RNNs, especially **LSTM and GRU**, can learn surprisingly nuanced patterns in character-level data across tasks like classification and generation.
* Text generation improves significantly with deeper layers and well-tuned hyperparameters.
* Language classification from character sequences is effective when using properly preprocessed and normalized text.

---

