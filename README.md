# Prompt Injection Detection in LLM-Integrated Applications
A machine learning and deep learning-based security system designed to detect and classify prompt injection attacks in user inputs before they reach a Large Language Model (LLM).

# Overview
Prompt injection attacks manipulate LLM behavior through malicious instructions embedded in inputs. This project implements a lightweight classifier placed in front of an LLM to categorize prompts as **Benign** or **Malicious**, with a strong emphasis on maintaining a low false-positive rate (FPR) to prevent disrupting legitimate users.

# Key Objectives
- Build a balanced, de-duplicated dataset incorporating various prompt injection attack patterns.
- Benchmark classical machine learning algorithms against deep learning and Transformer-based architectures.
- Evaluate models using Accuracy, Precision, Recall, F1-score, and True Positive Rate (TPR) at low False Positive Rates (0.1%–1% FPR).
- Propose a defense architecture combining real-time classification, risk scoring, and rate-limiting.

# Models Evaluated
- Random Forest
- Multinomial Naive Bayes
- Feed-Forward Neural Network (FNN)
- Long Short-Term Memory (LSTM)
- BERT (Transformer-based)

# Datasets
Publicly sourced datasets including HackAPrompt, SQuAD, Alpaca, and Databricks-Dolly, processed through custom cleaning, de-duplication, and balancing pipelines.

## Proposed Architecture
1. **User Prompt** enters the system.
2. **Prompt Injection Detector** analyzes the input.
3. **Classification:** If classified as *Benign*, it proceeds to the **LLM**. If *Malicious*, it triggers risk scoring/rate-limiting.

# Authors
- Atiya Srivastava
- Zoha Eajaz Shaikh
- Afreen Kazmi

# Academic Context
Software Engineering Project  
Department of Computer Science (Cyber Security)  
SVKM's NMIMS, Mukesh Patel School of Technology Management & Engineering  
Academic Year: 2026–2027
