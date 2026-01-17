# 💳 Generative AI–Enhanced Credit Card Fraud Detection & Analytics Platform

## 🚀 Executive Summary

This project presents an **end-to-end, production-inspired fraud detection and analytics system** that combines **classical machine learning**, **synthetic data generation using Large Language Models (LLMs)**, and a **Natural Language → SQL → Visualization assistant**.

Built on a **1.3M+ transaction synthetic dataset**, the system demonstrates how modern financial institutions can:

* Detect rare and evolving fraud patterns
* Reduce false positives while maintaining high recall
* Preserve user privacy using synthetic data
* Enable non-technical stakeholders to query fraud data using natural language

This repository reflects **industry-grade thinking**, not just model building.

---

## ❓ Why Credit Card Fraud Detection Matters

### 🌍 Real-World Impact

* Global card fraud causes **billions of dollars in losses annually**
* Fraud directly affects:

  * Banks & payment networks (financial loss)
  * Merchants (chargebacks)
  * Consumers (trust & credit score damage)

### ⚖️ Regulatory Pressure

* Compliance with **PCI-DSS, GDPR, and consumer protection laws** is mandatory
* Institutions must prove models are:

  * Accurate
  * Auditable
  * Explainable

### ⚠️ Key Challenge

Fraud data is:

* **Extremely imbalanced** (often <0.5% fraud)
* **Highly dynamic** (fraud patterns evolve)

➡️ Traditional rule-based systems fail to scale — motivating AI-driven solutions.

---

## 🧠 How Fraud Detection Works in Industry

Modern systems use **layered intelligence**:

1️⃣ **Rules Engine**
Simple heuristics (velocity checks, geo-mismatch)

2️⃣ **Machine Learning Models**
Learn complex, non-linear behavior patterns

3️⃣ **Behavioral Profiling**
Understand user-specific spending baselines

4️⃣ **Human Review Loop**
Analysts validate flagged transactions

📌 This project simulates **Layers 2–4** using ML + Generative AI.

---

## 🔐 Why Synthetic Data Is Essential

### 🚫 Why Real Data Is Not Public

* Contains PII and financial identifiers
* Protected by privacy laws
* Cannot be safely shared or open-sourced

### ✅ Why Synthetic Data Is Industry-Approved

* Preserves **statistical realism** without exposing identities
* Enables experimentation on rare fraud patterns
* Used by banks, regulators, and researchers

📚 Supported by literature on privacy-preserving fraud detection and class imbalance mitigation.

---

## 📊 Dataset Overview

* **Size:** ~1.3 million transactions
* **Time Range:** Dec 2018 – Jun 2020
* **Features Include:**

  * Transaction amount & timestamp
  * Merchant & category
  * Cardholder demographics
  * Location-based attributes
  * Fraud label (binary)

⚠️ Dataset reflects **real-world imbalance**, a core challenge addressed in this project.

---

## 🏗️ System Architecture

### Core Components

1. Classical ML Fraud Models
2. Synthetic Fraud Generation via LLMs
3. Fine-Tuned Language Model (LoRA)
4. NL → SQL → Visualization Assistant
5. Performance Comparison Engine (FPR-focused)

📌 Designed to mirror **modern fintech fraud pipelines**.

---

## 🤖 Machine Learning Models

### Baseline Models

* **Random Forest** (primary baseline)
* **Gradient Boosting**
* **Logistic Regression**

#### Why Random Forest?

* Handles mixed data types well
* Robust to noise & imbalance
* Strong baseline for tabular fraud data

---

## 📈 Evaluation Philosophy

### Why Accuracy Is Misleading

* 99% accuracy can still miss all fraud

### Metrics That Matter

* **Recall** → Catch fraud
* **False Positive Rate (FPR)** → Avoid blocking real customers
* **ROC-AUC** → Overall discrimination

📌 Industry prioritizes **low FPR with high recall**, not raw accuracy.

---

## 🧪 Feature Engineering & Bucketing

### Why Bucketing?

* Captures **non-linear risk tiers**
* Improves interpretability
* Mirrors real bank risk segmentation

Examples:

* Low amount → low risk
* Unusual mid-range → moderate risk
* Extremely high → elevated fraud probability

---

## 🧠 Synthetic Fraud Generation (LLM-Augmented)

### Motivation

* Fraud cases are rare
* Models underperform on unseen patterns

### Approach

* Convert user profiles into **textual behavior summaries**
* Fine-tune LLM using **LoRA adapters**
* Generate realistic fraudulent transactions
* Preserve feature distributions

📌 Synthetic augmentation **reduced false negatives and FPR** across models.

---

## 🗣️ Natural Language → SQL → Visualization Assistant

### What It Does

* Accepts natural language questions
* Generates optimized SQL
* Executes queries in **DuckDB**
* Produces visual insights automatically

### Example Questions

* “Which categories have the highest fraud rate?”
* “Show fraud trends by state.”
* “Compare daily fraud volume over time.”

📌 Enables **non-technical stakeholders** to explore fraud data.

---

## 🧰 Tools & Libraries

* **Python** (Core language)
* **Pandas / NumPy** (Data handling)
* **Scikit-learn** (ML models)
* **SHAP** (Explainability)
* **DuckDB** (Fast analytics)
* **Matplotlib / Seaborn / Plotly** (Visualization)
* **LLMs + LoRA** (Generative AI)

---

## 🔍 Explainability & Trust

* SHAP values explain feature contributions
* Improves transparency
* Supports regulatory compliance
* Builds stakeholder trust

📌 Explainability is **non-negotiable** in financial AI systems.

---

## 📉 Results Summary

* Synthetic augmentation improved fraud detection robustness
* Lowered False Positive Rates across models
* Enhanced model generalization to rare fraud patterns

📌 Demonstrates real value of Generative AI in tabular ML.

---

## 🚧 Limitations

* Synthetic data may not capture all real-world adversarial behavior
* Real-time streaming not implemented
* Cost-sensitive learning not fully explored

---

## 🔮 Future Enhancements

* Real-time Kafka/Spark pipeline
* Cost-aware loss functions
* API deployment
* Expanded economic indicators

---

## 👨‍💻 Authors

**Ajay Kumar**
Data Science Graduate | Machine Learning | Generative AI

Collaborators: Omkar Pardeshi, Ethan Pollock

---

## ⭐ Why This Project Matters

This repository demonstrates:

* End-to-end ML system thinking
* Ethical AI & privacy awareness
* Generative AI applied beyond text
* Real-world fraud detection trade-offs

If you’re a recruiter, this project shows how I **think**, not just how I code.
