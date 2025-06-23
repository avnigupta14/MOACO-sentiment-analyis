# MOACO for Sentiment Analysis 🚀
**Multi-Objective Ant Colony Optimization (MOACO) + LSTM** for real-time, large-scale sentiment classification on tweets.

This repository contains the official implementation of our research paper:

> **"From ACO to MOACO: Enhancing Sentiment Analysis via Multi-Objective Feature Selection and LSTM Networks"**  
> Avni Gupta-  Netaji Subhas University of Technology, Delhi, India  
---

## 🔍 Overview

Text-based sentiment analysis often suffers from high dimensionality and redundant features. We present **MOACO**, a novel algorithm that optimizes **both feature reduction and classification accuracy** using:

- Multi-objective Ant Colony Optimization (MOACO)
- Pareto frontier-based feature selection
- Deep LSTM-based classification

> 📊 Achieved:
> - 2.82% accuracy gain over traditional ACO
> - 65.7% fewer features
> - 37.5% faster training time
> - 44,800 additional correct predictions (on 1.6M tweets)

---

## 🧠 Core Components

| Component        | Description |
|------------------|-------------|
| `moaco.py`       | MOACO feature selector with Pareto archive and adaptive pheromone updates |
| `preprocess.py`  | Tweet cleaning, tokenization, stopword removal |
| `embedding.py`   | Word2Vec generation & PCA dimensionality reduction |
| `train_lstm.py`  | BiLSTM model with dropout, batch norm, Adam optimizer |
| `evaluate.py`    | Metrics: Accuracy, Precision, Recall, F1-score, Confusion Matrix |
| `notebooks/`     | Jupyter notebooks for experiment tracking & visualizations |

---
## 📊 Results

| Model | Accuracy | F1-Score | Features Used | Training Time |
|-------|----------|----------|----------------|----------------|
| ACO   | 62.15%   | 0.6389   | 350            | 12.8 hrs       |
| MOACO | 64.97%   | 0.6684   | 120            | 8 hrs          |

- ✅ **Memory reduced** from 4.2GB to 1.8GB
- ✅ **Inference 2.1× faster**
- ✅ **35% less GPU power consumption**

---
📂 Dataset
We use the Sentiment140 dataset (1.6M tweets).


