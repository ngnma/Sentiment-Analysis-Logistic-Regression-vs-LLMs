# 📊 Sentiment Analysis: Logistic Regression vs LLMs

A comparative study of **classical machine learning** and **large language models (LLMs)** for sentiment analysis. This project evaluates performance, efficiency, and practical trade-offs between **Logistic Regression with vectorization techniques** and **LLM-based prompting approaches**.

---

## 🚀 Overview

This repository investigates two fundamentally different paradigms for sentiment classification:

### 1. Traditional Machine Learning

* Logistic Regression (LR)
* Feature engineering techniques:

  * Bag of Words (BoW)
  * TF-IDF
  * Word2Vec
  * TF-IDF weighted Word2Vec

### 2. Large Language Models (LLMs)

* Instruction-tuned models (e.g., FLAN-T5)
* Prompt-based classification:

  * Zero-shot prompting
  * Rule-guided prompting
  * Few-shot prompting (optional)

The goal is to understand:

* When simpler models outperform LLMs
* How prompt design impacts LLM performance
* Trade-offs in **accuracy, interpretability, and computational cost**

---

## 🧠 Key Features

* End-to-end **sentiment analysis pipeline**
* Comparative analysis of **multiple vectorization techniques**
* **LLM prompting experiments** with controlled outputs
* Evaluation using:

  * Accuracy
  * F1-score (macro)
* Runtime and efficiency comparison
* Qualitative **error analysis and insights**

---

## 📊 Results Summary

The best-performing model was the **LLM-based approach**, achieving an **F1-score of 91.4%**, slightly outperforming **Logistic Regression (89.6%)**. Among the tested prompts, performance varied, highlighting the importance of prompt design.

| Model               | F1 Score  |
| ------------------- | --------- |
| Prompt 2            | **91.4%** |
| Prompt 1            | 91.0%     |
| Prompt 3            | 89.8%     |
| Prompt 4            | 89.0%     |
| Prompt 5            | 88.7%     |
| Logistic Regression | 89.6%     |

The results show that a well-designed prompt can outperform a traditional machine learning baseline. 

---

### Key Findings

* **Logistic Regression**

  * Performs strongly on short, explicit texts
  * Relies on keyword presence (e.g., “good”, “bad”)
  * Bag-of-Words achieved the best validation performance (~84%)

* **LLM-based Models**

  * More robust for longer and complex texts
  * Better at understanding context and sentence structure
  * Highly sensitive to prompt design

Overall, both approaches achieve strong performance, with LLMs offering a slight advantage when properly guided. 

---

## 🧪 Experiments

* Compared multiple feature representations for LR
* Evaluated prompt engineering strategies for LLMs
* Analyzed:

  * Misclassifications
  * Sensitivity to text length
  * Handling of contrastive phrases (e.g., “but”, “however”)

---

## 📌 Future Work

* Fine-tuning transformer models (e.g., BERT)
* Expanding datasets and domains
* Automating prompt optimization
* Hybrid models (ML + LLM)
