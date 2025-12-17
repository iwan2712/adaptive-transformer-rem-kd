# An Adaptive Transformer-Based Model with Entropy-Driven Knowledge Distillation  
## for Single-Channel EEG REM Sleep Detection

<p align="center">
  <b>Shih-Chung Chen</b>, <b>Irawan Dwi Wahyono</b><sup>*</sup><br>
  Department of Electrical Engineering, Southern Taiwan University of Science and Technology
</p>

---

## 📌 Overview
Accurate detection of **rapid eye movement (REM) sleep** is critical for neurophysiological monitoring and early identification of sleep-related disorders.  
This repository presents an **entropy-driven adaptive knowledge distillation framework** integrated with a **lightweight Transformer**, designed for **robust REM sleep detection from single-channel EEG signals**.

---

## ✨ Key Idea
🔹 **Why uncertainty-aware distillation?**  
REM sleep exhibits high inter-subject variability and ambiguous temporal patterns.  
To address this, we explicitly model uncertainty by dynamically adjusting:

- 🌡️ **Distillation temperature**
- ⚖️ **Loss weighting**

based on **teacher–student entropy alignment**.

This enables **better generalization**, especially under **subject-independent evaluation**.

---

## 🧪 Experimental Setup
- **Datasets**:
  - Sleep-EDF  
  - ISRUC-Sleep  
  - MASS  

- **Evaluation protocol**:
  - Subject-independent cross-validation
  - Cross-dataset generalization analysis

- **Baselines**:
  - CNN
  - LSTM
  - Standard Transformer

---

## 📊 Results (Highlights)
| Model | Accuracy | F1-score |
|------|---------|---------|
| CNN | 85.2% | 83.6% |
| LSTM | 88.5% | 87.4% |
| Transformer | 92.3% | 91.8% |
| **Proposed (Adaptive KD)** | **93.2%** | **92.8%** |

✅ **~30% reduction** in training time and memory usage  
✅ Suitable for **real-time** and **wearable EEG applications**

---

## Abstract
Accurate detection of rapid eye movement (REM) sleep is critical for neurophysiological monitoring and early identification of sleep-related disorders.  
We propose an **entropy-driven adaptive knowledge distillation framework** integrated with a lightweight Transformer to enable robust REM sleep detection from **single-channel EEG signals**. By dynamically adjusting temperature scaling and distillation weighting based on teacher–student entropy, the proposed approach explicitly models uncertainty inherent in REM sleep.  

Evaluated under subject-independent cross-validation on three public datasets (Sleep-EDF, ISRUC-Sleep, and MASS), the proposed model consistently outperforms CNN, LSTM, and standard Transformer baselines, achieving an average accuracy of **93.2%** and an F1 score of **92.8%**. Moreover, the distilled student model reduces training time and memory usage by approximately **30%**, supporting efficient deployment in real-time and wearable EEG applications.

---

## 🔑 Keywords
`REM sleep` · `Electroencephalogram (EEG)` · `Knowledge Distillation` · `Transformer` · `Sleep Staging`

---

