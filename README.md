# Supervised-Contrastive-Learning-with-Attention-Emotion-Synthesis-for-Implicit-Hate-Speech-Detection

This repository contains the implementation and resources for the research paper titled *"Leveraging Supervised Contrastive Learning with Attention Mechanisms and Emotion Synthesis for Detecting Implicit Hate Speech"* by *Sri Akash Kadali* and *Harshith Chejerla*.

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

| Dataset     | Metric    | BERT  | DeBERTa | Proposed Method |
|-------------|-----------|-------|---------|-----------------|
| IHate       | F1-Score  | 83.3  | 88.2    | *89.8*        |
| IHate       | Accuracy  | 85.9  | 87.6    | *89.9*        |
| IHC         | F1-Score  | 77.2  | 79.1    | *82.6*        |

---

## 🛠 Installation

To run this project locally:

1. Clone the repository:
   ```bash
   git clone [(https://github.com/Akash-Kadali/Supervised-Contrastive-Learning-with-Attention-Emotion-Synthesis-for-Implicit-Hate-Speech-Detection.git)]
## 📂 Repository Structure
