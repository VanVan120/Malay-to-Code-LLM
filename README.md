# 🇲🇾 Malay-to-Code: Fine-Tuning LLMs for Bahasa Melayu Programming

[![Project Status: Research](https://img.shields.io/badge/status-research-blue)]()
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)]()

A research initiative to fine-tune a Large Language Model (LLM) for generating programming code from natural language commands in Bahasa Melayu (Malay).

---

## 💡 Project Overview

This project successfully bridged the linguistic gap in AI-driven software development by creating and training on a novel, high-quality dataset of programming prompts in Bahasa Melayu. We fine-tuned a large language model (LLM) using **85,371 programming prompts** across various programming languages translated to Malay, and benchmarked the model's performance specifically on **Python programming tasks** to measure improvements over baseline models.

---

## 🤔 The Problem

Most large language models are trained predominantly on English text. As a result, non-English speaking communities—like those who use Bahasa Melayu—face significant challenges using these models, as they often struggle to understand and generate code from prompts in other languages.

---

## ✅ Our Solution

We successfully localized LLM capabilities for Bahasa Melayu by:

- **Generated a Multi-Language Dataset:** Created a comprehensive dataset of **85,371 programming prompts** by machine-translating common English programming prompts covering various languages (Python, JavaScript, SQL, etc.) into Bahasa Melayu.
- **Validated the Dataset:** Applied quality filtering and validation techniques using semantic similarity scores to ensure translations maintain technical accuracy and clarity.
- **Fine-Tuned the Model:** Successfully trained a large language model using the complete validated dataset of 85,371 Malay programming prompts spanning multiple programming languages.
- **Evaluated Performance on Python:** Rigorously tested and benchmarked the fine-tuned model specifically on **Python programming tasks** using the HumanEval-XL dataset (80 problems) to measure improvements over baseline models.

---

## 🛠️ Methodology: Completed Research

### 1. Data Generation & Translation ✅

- Successfully processed and translated **85,371 programming prompts** from English to Malay using automated translation tools.
- The dataset covers multiple programming languages including Python, JavaScript, SQL, and others.
- Applied comprehensive data cleaning and preprocessing techniques.

### 2. Dataset Quality Validation ✅

- Implemented semantic similarity scoring using BERTScore and other metrics to validate translation quality.
- Applied filtering techniques to ensure only high-quality translations (F1 scores above threshold) were included in the final training set.
- Achieved a robust dataset suitable for language model fine-tuning.

### 3. Fine-Tuning & Evaluation ✅

- **Training:** Successfully fine-tuned the LLM using the complete dataset of **85,371 multi-language programming prompts** in Bahasa Melayu.
- **Evaluation Focus:** Conducted comprehensive benchmarking specifically on **Python programming tasks** to measure the model's code generation capabilities.
- **Benchmark Dataset:** Used the HumanEval-XL evaluation framework with **80 Python programming problems** available in both English and Malay.
- **Performance Analysis:** Compared pre-training vs. post-training performance to quantify improvements in understanding Malay programming instructions for Python code generation.

---

## 📊 Dataset & Results

### Training Dataset
- **Size:** 85,371 programming prompts
- **Languages:** Multiple programming languages (Python, JavaScript, SQL, etc.)
- **Translation:** English to Bahasa Melayu using automated translation with quality validation
- **Quality Control:** Semantic similarity filtering and BERTScore validation

### Evaluation Dataset  
- **Framework:** HumanEval-XL
- **Focus:** Python programming tasks only
- **Size:** 80 coding problems
- **Languages:** Available in both English and Malay for comparison

### Key Findings
- Successfully trained a multilingual code LLM on diverse programming languages in Malay
- Benchmarked specifically on Python to demonstrate effectiveness of Malay instruction understanding
- Demonstrated measurable improvements in code generation from Malay natural language instructions

---

## 🤝 Future Collaboration

This research demonstrates the successful fine-tuning of LLMs for Bahasa Melayu programming tasks. We welcome further collaboration to:

- Extend evaluation to other programming languages beyond Python
- Expand the training dataset with more diverse programming domains
- Explore advanced fine-tuning techniques and model architectures  
- Conduct comparative studies with other multilingual code models

**Interested in collaboration?** Reach out to us via email (see below). Contributors will be acknowledged in future publications.

---

## ✉️ Contact Us

**Ivan Char Cheng Jun, hfyic3@nottingham.edu.my**  
University of Nottingham Malaysia

**Cham Jin Jie, hfyjc23@nottingham.edu.my**  
University of Nottingham Malaysia

**Supervisor:** Dr. Simon Lau Boung Yew, simon.lau@nottingham.edu.my  
School of Computer Science, University of Nottingham Malaysia

---

Thank you for your interest in supporting AI localization for Bahasa Melayu and making programming more accessible for everyone!
