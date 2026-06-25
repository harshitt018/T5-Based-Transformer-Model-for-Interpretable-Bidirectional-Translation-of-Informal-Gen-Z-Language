# 🧠 T5-Based Gen-Z Slang Translation using Transformer

<p align="center">

<a href="https://iaraedu.com/about-journal/ijair-volume-13-issue-1-xiii-january-march-2026.php">
<img src="https://img.shields.io/badge/Published-IJAIR%20Vol.13%20Issue%201%20(XIII)-blue">
</a>

<a href="https://zenodo.org/records/20354105">
<img src="https://img.shields.io/badge/DOI-10.5281%2Fzenodo.20354105-blue">
</a>

<img src="https://img.shields.io/badge/ISSN-2394--7780-orange">

<img src="https://img.shields.io/badge/SJIF%20Impact%20Factor-8.12-success">

<img src="https://img.shields.io/badge/NLP-Transformer-green">

<img src="https://img.shields.io/badge/T5-Model-red">

<img src="https://img.shields.io/badge/Python-3.9+-3776AB?logo=python&logoColor=white">

</p>


</p>

An interpretable Transformer-based framework for bidirectional translation between Standard English and Gen-Z slang using a fine-tuned T5 model, lexical augmentation, and attention-based explainability. Designed to bridge communication gaps between generations while preserving meaning, intent, and conversational context.

This repository accompanies the peer-reviewed research paper **"A T5-Based Transformer Model for Interpretable Bidirectional Translation of Informal Gen-Z Language"**, published in the **International Journal of Advance and Innovative Research (IJAIR), Volume 13, Issue 1 (XIII), January–March 2026**.

---

## 📄 Research Publication

### Paper Title

**A T5-Based Transformer Model for Interpretable Bidirectional Translation of Informal Gen-Z Language**

**Journal:** International Journal of Advance and Innovative Research (IJAIR)

**Volume:** 13

**Issue:** 1 (XIII)

**Publication Period:** January – March 2026

**Pages:** 292–302

**DOI:** https://zenodo.org/records/20354105

**Journal Link:** https://iaraedu.com/about-journal/ijair-volume-13-issue-1-xiii-january-march-2026.php

**Conference Presentation:** ICMVLU 2026 (28 February 2026)

---

## 📌 Overview

Developments in Natural Language Processing (NLP) have highlighted the growing need to process informal digital language. However, understanding and translating rapidly evolving Gen-Z slang remains a challenging task due to changing expressions, social context, and linguistic variation.

This research introduces a bidirectional translation framework based on a fine-tuned Text-to-Text Transfer Transformer (T5) model trained on an expanded English–Gen-Z parallel corpus. Unlike traditional rule-based approaches, the proposed system treats slang translation as a text generation task, allowing the model to preserve semantic meaning while adapting stylistic expressions.

The framework incorporates lexical augmentation, normalization strategies, and attention-based explainability mechanisms to improve translation quality and interpretability.

---

## ✨ Key Features

* Bidirectional Translation (English ↔ Gen-Z)
* Fine-Tuned T5-Small Transformer Architecture
* Context-Aware Slang Understanding
* Lexical Augmentation for Controlled Slang Generation
* Lexical Normalization for Gen-Z → English Translation
* Attention-Based Explainability
* BLEU Score Evaluation
* Semantic Similarity Analysis
* Low-Resource NLP Research
* Explainable AI for Informal Language Processing

---

## 🏗️ Architecture

**Pipeline:** `Input Sentence → SentencePiece Tokenizer → T5 Encoder → T5 Decoder → Post Processing → Explainability Layer → Final Translation`

```text
Input: English Sentence / Gen-Z Slang Sentence

├── SentencePiece Tokenizer
│
├── T5 Encoder
│   ├── Multi-Head Attention
│   ├── Feed-Forward Network
│   └── Layer Normalization
│
├── T5 Decoder
│   ├── Masked Self-Attention
│   ├── Cross-Attention
│   └── Feed-Forward Network
│
├── Post Processing Layer
│   ├── Lexical Augmentation (English → Gen-Z)
│   └── Lexical Normalization (Gen-Z → English)
│
├── Explainability Module
│   ├── Word-Level Mapping
│   ├── Transformation Tracking
│   └── Translation Explanation
│
└── Final Translated Output
```

- **Model Architecture:** T5-Small Transformer (Encoder–Decoder)
- **Translation Type:** Bidirectional (English ↔ Gen-Z)
- **Tokenizer:** SentencePiece Subword Tokenization
- **Optimization:** AdamW Optimizer
- **Loss Function:** Cross-Entropy Loss
- **Evaluation Metrics:** BLEU Score, Semantic Similarity Analysis
- **Interpretability:** Explainability Layer with Word-Level Transformations
---

## 📊 Results

### Translation Performance

| Metric                | Value                 |
| --------------------- | --------------------- |
| BLEU Score            | 0.43                  |
| Model Architecture    | T5-Small Transformer  |
| Dataset Size          | ~3,000 Sentence Pairs |
| Translation Direction | English ↔ Gen-Z       |
| Training Epochs       | 5                     |
| Batch Size            | 8                     |
| Learning Rate         | 5e-5                  |

### Key Outcomes

✅ Improved translation quality compared to rule-based normalization systems

✅ Preserved semantic meaning and conversational intent

✅ Consistent slang generation and normalization

✅ Bidirectional translation capability

✅ Explainable and interpretable translation process

---

## 🧠 Tech Stack

<p align="center">

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>

<img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black"/>

<img src="https://img.shields.io/badge/Transformers-FF6F00?style=for-the-badge"/>

<img src="https://img.shields.io/badge/T5-Transformer-E53935?style=for-the-badge"/>

<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"/>

<img src="https://img.shields.io/badge/SentencePiece-Tokenizer-2196F3?style=for-the-badge"/>

<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>

<img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white"/>

<img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white"/>

<img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge"/>

</p>

---

## 🎯 Dataset

### Gen-Z Slang Sentence Pairs Dataset

Dataset Source:

https://www.kaggle.com/datasets/programmerrdai/genz-slang-pairs-1k

Dataset Statistics:

* Original Dataset: ~1,000 Sentence Pairs
* Expanded Dataset: ~3,000 Sentence Pairs
* Language: English ↔ Gen-Z Slang
* Format: Parallel Text Corpus

Example:

| Standard English          | Gen-Z Slang                |
| ------------------------- | -------------------------- |
| This movie is very good   | This movie is fire         |
| I am really tired today   | I'm dead today             |
| My friend is coming later | My bro is pulling up later |

---

## 📖 Citation

If you use this work, please cite:

```bibtex
@article{jaiswal2026t5genz,
  title={A T5-Based Transformer Model for Interpretable Bidirectional Translation of Informal Gen-Z Language},
  author={Jaiswal, Harshit and Tripathi, Sumitkumar and Kanojia, Mahendra},
  journal={International Journal of Advance and Innovative Research},
  volume={13},
  number={1 (XIII)},
  year={2026},
  issn={2394-7780},
  doi={10.5281/zenodo.20354105}
}
```

---

## 🔭 Future Work

* Real-Time Slang Adaptation
* Larger Multilingual Slang Corpora
* Advanced Explainability Techniques
* Mobile and Web Deployment
* Conversational AI Integration
* Continual Learning for Emerging Slang

---

## 👥 Authors

### Harshit Jaiswal

Information Technology
Sheth L.U. Jhaveri & Sir M.V. College, Mumbai

### Sumitkumar Tripathi

Information Technology
Sheth L.U. Jhaveri & Sir M.V. College, Mumbai

### Dr. Mahendra K. Kanojia

Department of Computer Science
Sheth L.U. Jhaveri & Sir M.V. College, Mumbai

---

## 🙏 Acknowledgement

The authors sincerely thank the Department of Information Technology, Sheth L.U. Jhaveri College of Arts and Sir M.V. College of Science and Commerce, Mumbai, for providing academic guidance, research support, and resources that contributed to the successful completion of this research work.

Special thanks to **Mr. Sumit Tripathi Sir** and **Dr. Mahendra K. Sir** for their continuous guidance, mentorship, and encouragement throughout this research journey.

---

## 📄 License

This project is intended for academic and research purposes. Please contact the corresponding author regarding reuse of trained models, datasets, or research materials.


---

## ✍️ Author

Harshit Jaiswal
