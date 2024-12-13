# Supervised-Contrastive-Learning-with-Attention-Emotion-Synthesis-for-Implicit-Hate-Speech-Detection

This repository contains the implementation and resources for the research paper titled *"Leveraging Supervised Contrastive Learning with Attention Mechanisms and Emotion Synthesis for Detecting Implicit Hate Speech"* by *Sri Akash Kadali*.

## 📜 Abstract

Implicit hate speech detection faces significant challenges due to its subtle and indirect nature, often disguised as humor, sarcasm, or indirect references. This project proposes a novel framework leveraging *supervised contrastive learning* with *attention mechanisms* and *emotion synthesis* to detect implicit hate speech. It focuses on augmenting datasets, extracting emotional context, and incorporating state-of-the-art transformer models.

---

## 🚀 Features

- *Supervised Contrastive Learning:* Enhances classification by utilizing contrastive losses for better feature representations.
- *Emotion Synthesis:* Adds emotional dimensions to text, capturing sentiment cues to improve model performance.
- *Attention Mechanisms:* Leverages Bi-LSTM and word-level attention for contextual understanding.
- *Extensive Data Augmentation:* Employs various augmentation strategies to enrich training datasets.
- *State-of-the-art Models:* Utilizes robust transformer models like DeBERTa for feature extraction and classification.

---
---

## 📊 Methodology

The proposed solution comprises the following steps:

1. *Data Preprocessing:* Clean datasets by removing noise, special characters, and redundant information.
2. *Data Augmentation:*
   - Replace Named Entities (RNE)
   - Replace Scalar Adverbs (RSA)
   - Back Translation (BT)
   - Generative Models (GM)
3. *Feature Extraction:*
   - Utilize *DeBERTa* for contextual embeddings.
   - Incorporate *sentiment and emotion features* via NRC Lexicon.
4. *Attention Mechanisms:*
   - Employ *Bi-LSTM* and *word-level attention* for contextual understanding.
5. *Contrastive Learning:*
   - Implement *Supervised Contrastive Loss (SupConLoss)* for improved feature representation.

![System Architecture](path/to/system_architecture_image.png)

---

## 📊 Results

The proposed method was evaluated on the *IHSate* and *IHC* datasets using metrics such as Accuracy, Precision, Recall, and F1-Score. It achieved significant improvements over baseline models like BERT, DeBERTa, and others.
# Model Performance Comparison

This document presents a comparison of model performance metrics for various models evaluated on two datasets.

## Dataset 1: Performance Metrics

| Model              | Precision | Recall   | F1 Score | Precision | Recall   | F1 Score | Precision | Recall  | F1 Score | Accuracy |
|--------------------|-----------|----------|----------|-----------|----------|----------|-----------|---------|----------|----------|
| **BERT**           | 0.888     | 0.902    | 0.895    | 0.813     | 0.811    | 0.812    | 0.469     | 0.37    | 0.414    | 0.848    |
| **HateBERT**       | 0.892     | 0.894    | 0.892    | 0.811     | 0.815    | 0.813    | 0.382     | 0.349   | 0.365    | 0.843    |
| **Roberta**        | 0.902     | 0.902    | 0.902    | 0.823     | 0.843    | 0.833    | 0.427     | 0.344   | 0.381    | 0.857    |
| **USE+SVM**        | 0.891     | 0.862    | 0.872    | 0.761     | 0.809    | 0.783    | 0.402     | 0.361   | 0.382    | 0.82     |
| **DeBERTa**        | 0.901     | 0.9      | 0.9      | 0.822     | 0.835    | 0.828    | 0.416     | 0.371   | 0.392    | 0.855    |
| **HateBERT+ALL**   | 0.903     | 0.896    | 0.899    | 0.827     | 0.827    | 0.827    | 0.502     | 0.559   | 0.529    | 0.84     |
| **USE+TFIDF**      | 0.82      | 0.918    | 0.866    | 0.785     | 0.709    | 0.745    | 0.667     | 0.043   | 0.081    | 0.816    |
| **USE+Count Vectorizer** | 0.834 | 0.872    | 0.853    | 0.741     | 0.718    | 0.73     | 0.321     | 0.194   | 0.242    | 0.79     |
| **LSTM-based Comparative** | 0.85 | 0.815    | 0.832    | 0.773     | 0.636    | 0.698    | 0.103     | 0.312   | 0.155    | 0.732    |
| **Bi-CHAT Model**  | 0.853     | 0.826    | 0.84     | 0.725     | 0.733    | 0.733    | 0.24      | 0.253   | 0.246    | 0.776    |
| **Paper 2 Published** | 0.9    | 0.9      | 0.9      | 0.81      | 0.85     | 0.83     | 0.45      | 0.82    | 0.58     | Did Not Mention |
| **Our Model**      | 0.891    | 0.918    | 0.904    | 0.816     | 0.865    | 0.84     | 0.608     | 0.579   | 0.593    | 0.863    |

## Dataset 2: Performance Metrics

| Model              | Precision | Recall   | F1 Score | Precision | Recall   | F1 Score | Precision | Recall  | F1 Score | Accuracy | Implicit Accuracy |
|--------------------|-----------|----------|----------|-----------|----------|----------|-----------|---------|----------|----------|-------------------|
| **BERT**           | 0.827     | 0.829    | 0.828    | 0.635     | 0.656    | 0.645    | 0.512     | 0.386   | 0.441    | 0.751    |                   |
| **HateBERT**       | 0.817     | 0.836    | 0.827    | 0.624     | 0.632    | 0.638    | 0.538     | 0.343   | 0.419    | 0.745    |                   |
| **Roberta**        | 0.816     | 0.844    | 0.83     | 0.641     | 0.631    | 0.636    | 0.509     | 0.344   | 0.41     | 0.75     |                   |
| **USE+SVM**        | 0.829     | 0.739    | 0.777    | 0.549     | 0.681    | 0.612    | 0.333     | 0.312   | 0.322    | 0.7      |                   |
| **DeBERTa**        | 0.818     | 0.826    | 0.822    | 0.621     | 0.634    | 0.627    | 0.474     | 0.344   | 0.398    | 0.741    |                   |
| **HateBERT+ALL**   | 0.812     | 0.802    | 0.807    | 0.709     | 0.765    | 0.745    | 0.503     | 0.723   | 0.593    |          |                   |
| **USE+TFIDF**      | 0.746     | 0.875    | 0.805    | 0.614     | 0.489    | 0.545    | 0.826     | 0.117   | 0.204    | 0.713    |                   |
| **USE+Count Vectorizer** | 0.745 | 0.818    | 0.78     | 0.553     | 0.493    | 0.521    | 0.372     | 0.178   | 0.241    | 0.681    |                   |
| **LSTM-based Comparative** | 0.756 | 0.708  | 0.731    | 0.475     | 0.54     | 0.505    | 0.253     | 0.233   | 0.243    | 0.63     |                   |
| **Bi-CHAT Model**  | 0.76      | 0.68     | 0.717    | 0.463     | 0.589    | 0.518    | 0.284     | 0.166   | 0.209    | 0.624    |                   |
| **Paper**          |           |          |          |           |          |          | 58.6      | 59.1    | 58.6     |          | 63.8             |
| **Our Model**      |           |          |          | 0.549     | 0.73     | 0.627    |           |         |          |          | 67.2             |

---

## 🛠 Installation

To run this project locally:

1. Clone the repository:
   ```bash
   git clone [(https://github.com/Akash-Kadali/Supervised-Contrastive-Learning-with-Attention-Emotion-Synthesis-for-Implicit-Hate-Speech-Detection.git)]
## 📂 Repository Structure
