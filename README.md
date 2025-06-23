# MOACO for Sentiment Analysis 
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

## 📁 Files Included

| File | Description |
|------|-------------|
| `moaco_code.ipynb` | Main Jupyter notebook with MOACO implementation and sentiment analysis using LSTM |
| `aco_code.ipynb` | Baseline notebook using standard ACO for feature selection |
| `moaco_paper.pdf` | Final research paper detailing our methodology, experiments, and results |

---

 ## 📊 Run the notebooks

- Open moaco_code.ipynb in Jupyter or VS Code
- Download the Sentiment140 dataset and place it in the same folder 
- Follow the steps in the notebook for preprocessing, feature selection, and model training



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


