# 🇲🇾 Malay-to-Code-LLM: Advancing Code Generation for Bahasa Melayu

[![Project Status: Research](https://img.shields.io/badge/status-research%20complete-brightgreen)](https://github.com/VanVan120/Malay-to-Code-LLM)
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Dataset: 1M+ Entries](https://img.shields.io/badge/dataset-1M%2B%20entries-blue)]()
[![Languages: 12+](https://img.shields.io/badge/programming%20languages-12%2B-orange)]()
[![University: Nottingham Malaysia](https://img.shields.io/badge/university-Nottingham%20Malaysia-red)](https://www.nottingham.edu.my/)

> **🏆 A groundbreaking research initiative that successfully developed the first large-scale parallel dataset for Bahasa Melayu code generation, advancing multilingual programming language models for Southeast Asian developers.**

---

## 📊 Project Highlights

- **🗃️ 1,000,000+** processed training entries across multiple dataset variants
- **🌍 12 Programming Languages** evaluated via HumanEval-XL benchmark
- **📈 Translation Quality Score** Average BERTScore F1: 0.41, COMET evaluation on 3,400+ samples
- **🔧 Complete Pipeline** From data processing to model evaluation
- **🏫 Academic Research** University of Nottingham Malaysia Computer Science Department

---

## 🌟 What Makes This Project Special

### 🎯 **First-of-its-Kind Dataset**
This repository contains the **world's first comprehensive parallel dataset** for Bahasa Melayu programming instruction translation, bridging the gap between English-dominant AI models and Malay-speaking developers.

### 🔬 **Rigorous Evaluation Framework**
- **BERTScore Evaluation**: Semantic similarity assessment between English and Malay translations
- **COMET Scoring**: Advanced machine translation quality metrics
- **Multi-language Testing**: Comprehensive evaluation across 12 programming languages
- **Human Validation**: Expert linguistic review and quality assurance

### 🛠️ **Complete Research Pipeline**
From raw data processing to final model evaluation, this repository documents the entire research methodology with reproducible results.

---

## 📈 Dataset Overview

| Dataset Component | Size | Description |
|------------------|------|-------------|
| **Original Dataset** | 85,371 entries | Base English programming instructions |
| **Processed Training Data** | 1,000,000+ entries | Multiple variants with quality filtering |
| **Final Malay Translations** | Complete coverage | High-quality Bahasa Melayu translations |
| **Evaluation Results** | 3,400+ samples | BERTScore and COMET quality metrics |

### 🎨 **Programming Languages Covered**
`Python` • `JavaScript` • `Java` • `C#` • `Go` • `PHP` • `Ruby` • `Swift` • `Kotlin` • `Scala` • `TypeScript` • `Perl`

---

## 🔧 Technical Implementation

### **🤖 Core Technologies**
- **Base Dataset**: `iamtarun/code_instructions_120k_alpaca` (HuggingFace)
- **Translation Model**: Google Translate API integration
- **Semantic Evaluation**: SentenceTransformers with LaBSE multilingual model
- **Quality Assessment**: BERTScore and COMET evaluation frameworks
- **Benchmark**: HumanEval-XL for multi-language code generation

### **📊 Data Processing Pipeline**
```
Raw English Instructions → Translation → Quality Filtering → Expert Validation → Final Dataset
     (85K entries)         (1M+ variations)  (Score-based)    (Human review)    (Production-ready)
```

### **🎯 Quality Metrics**
- **BERTScore F1**: 0.41 average semantic similarity
- **COMET Score**: Comprehensive translation quality evaluation
- **Score-based Filtering**: Multiple quality tiers (>0.3, >0.7 thresholds)
- **Semantic Similarity**: LaBSE-based cosine similarity assessment

---

## 📁 Repository Structure

```
Malay-to-Code-LLM/
├── 📓 data_manipulation.ipynb           # Complete data processing pipeline
├── 📊 bertscore_results/               # BERTScore evaluation outputs
├── 🎯 comet_results/                   # COMET translation quality scores
├── 🗃️ original datasets/              # Base English programming instructions
├── 🔄 cleaned_train seperation/       # Processed training data variants
├── ✅ final_train seperation/         # Production-ready translated datasets
├── 📈 Score seperation/               # Quality-filtered dataset variants
├── 🧪 Evaluation dataset HumanEval-XL/ # Multi-language benchmark suite
├── 🎲 interleaving every 10 good datas 1 bad data/ # Data quality experiments
├── 📋 eng+ms_train.jsonl              # English-Malay parallel training data
├── 📄 Summer Internship Report.pdf    # Comprehensive research documentation
└── 📜 LICENSE                         # MIT License
```

---

## 🚀 Getting Started

### **Prerequisites**
```bash
# Install required packages
pip install datasets transformers torch
pip install sentence-transformers
pip install bert-score comet-ml
```

### **Data Processing**
```bash
# Load and explore the main dataset
import json
with open('eng+ms_train.jsonl', 'r', encoding='utf-8') as f:
    data = [json.loads(line) for line in f]
    
print(f"Dataset size: {len(data)} entries")
print(f"Sample: {data[0]}")
```

### **Evaluation**
```bash
# Run semantic similarity evaluation
from sentence_transformers import SentenceTransformer
model = SentenceTransformer('sentence-transformers/LaBSE')

# Evaluate translation quality
python evaluate_bertscore.py --input final_train.jsonl --output results.jsonl
```

---

## 📊 Key Research Findings

### **🎯 Translation Quality Distribution**
- **High Quality (F1 > 0.7)**: Premium translations for critical applications
- **Medium Quality (F1 0.3-0.7)**: Suitable for general training purposes  
- **Filtered Dataset**: Quality-based separation for targeted model training

### **🌐 Multilingual Impact**
This research demonstrates the feasibility of creating high-quality parallel datasets for underrepresented languages in programming AI, opening doors for similar initiatives across Southeast Asian languages.

### **📈 Evaluation Insights**
- Semantic similarity preservation across language barriers
- Context-aware translation maintaining programming logic
- Scalable methodology applicable to other language pairs

---

## 🎓 Academic Contribution

This project represents a **significant contribution to multilingual NLP research**:

- **Novel Dataset**: First comprehensive Malay programming instruction dataset
- **Methodology**: Reproducible pipeline for similar language pairs
- **Evaluation Framework**: Comprehensive quality assessment methodology
- **Open Source**: Complete codebase and data for community advancement

---

## 🤝 Research Collaboration

### **How to Contribute**
- **📊 Data Validation**: Review translation quality and suggest improvements
- **🔬 Model Training**: Fine-tune LLMs using our datasets
- **📈 Evaluation**: Extend benchmarks to additional programming languages
- **📚 Research**: Cite and build upon our methodology

### **Publication & Recognition**
Contributors are formally acknowledged in research publications. This work advances the state-of-the-art in multilingual code generation.

---

## 📖 Citation

If you use this dataset or methodology in your research, please cite:

```bibtex
@misc{malay-to-code-llm-2024,
  title={Malay-to-Code-LLM: Fine-Tuning Large Language Models for Bahasa Melayu Programming},
  author={Ivan Char Cheng Jun and Cham Jin Jie and Simon Lau Boung Yew},
  year={2024},
  institution={University of Nottingham Malaysia, School of Computer Science},
  url={https://github.com/VanVan120/Malay-to-Code-LLM}
}
```

---

## 👥 Research Team

**🎓 Students**
- **Ivan Char Cheng Jun** - Lead Researcher  
  📧 hfyic3@nottingham.edu.my

- **Cham Jin Jie** - Data Science & Evaluation  
  📧 hfyjc23@nottingham.edu.my

**👨‍🏫 Supervisor**
- **Dr. Simon Lau Boung Yew** - Principal Investigator  
  📧 simon.lau@nottingham.edu.my  
  🏫 School of Computer Science, University of Nottingham Malaysia

---

## 🏆 Impact & Future Work

This research **bridges the digital divide** by making programming AI more accessible to Malay-speaking developers, contributing to:

- **🌍 Digital Inclusion**: Democratizing AI-assisted programming
- **🎓 Educational Access**: Supporting computer science education in Malaysia
- **💼 Industry Applications**: Enabling localized development tools
- **🔬 Research Advancement**: Foundation for future multilingual AI research

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<div align="center">

### 🇲🇾 **Membangun Masa Depan Pengaturcaraan dalam Bahasa Melayu**
### **Building the Future of Programming in Malay**

*Thank you for supporting AI localization and making programming more accessible for everyone!*

[![University of Nottingham Malaysia](https://img.shields.io/badge/🏫-University%20of%20Nottingham%20Malaysia-red)](https://www.nottingham.edu.my/)

</div>
