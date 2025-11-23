# 🌍 Climate Strategy Generation using LLMs

### **Fine-Tuning T5 on Climate TRACE Dataset for Emission Reduction Recommendations**

This project develops a domain-specialized **Large Language Model** capable of generating **emission-reduction strategies** for industrial facilities using real climate data. The model is fine-tuned on the official **Climate TRACE – Top Emission Reduction Strategies** dataset, enabling intelligent, sector-specific, and actionable sustainability recommendations.

---

## 🚀 Project Overview

The goal is to train a model that can:

* Understand structured facility metadata
* Generate context-specific emission reduction strategies
* Assist in Net-Zero transition planning
* Provide climate action recommendations for industries

You achieve this by fine-tuning **T5-small** on 3,000 curated examples from the 1M-row Climate TRACE dataset.

---

## 📈 Key Results

| Metric      | Score |
| ----------- | ----- |
| **ROUGE-1** | 0.71  |
| **ROUGE-L** | 0.70  |
| **BLEU**    | 45+   |

These results show **strong learning of domain-specific sustainability knowledge**, outperforming the base T5 model significantly.

---

## 🧠 Features

* 🔹 End-to-end fine-tuning pipeline
* 🔹 Real Climate TRACE dataset preprocessing
* 🔹 LLM training using Hugging Face Transformers
* 🔹 Evaluation using ROUGE & BLEU metrics
* 🔹 Comparison of **base vs fine-tuned T5**
* 🔹 Clean inference scripts
* 🔹 All steps implemented in Jupyter Notebook

---

## 🧪 Sample Input → Output

### **Input**

```
Facility: Sunndalsora aluminium plant | 
Country: NOR | 
Sector: aluminum | 
EmissionReductionPotential(Mt): 0.78 | 
Difficulty: Short-term
```

### **Fine-Tuned Model Output**

```
Short-term strategy: Increase recycled aluminum feedstock to reduce alumina demand and cut CO₂ emissions.
Mid-term strategy: Optimize smelting energy efficiency and integrate low-carbon power sources.
Long-term strategy: Transition to renewable-intensive smelting and advanced low-emission technologies.
```

---

## 🧱 Repository Structure

```
📁 Climate-Strategy-LLM/
│
├── result images
├── processed_data/                      # Cleaned train/val/test CSVs
│   ├── train.csv
│   ├── val.csv
│   └── test.csv
│
├── climate_finetuning.ipynb             # Main fine-tuning pipeline
│
├── t5_climate_strategy_final/           # Saved fine-tuned model
│
└── README.md                            # Project documentation (this file)
```

---

## 🛠️ Tech Stack

* **Python**
* **Hugging Face Transformers**
* **T5-small (Seq2Seq LLM)**
* **PyTorch**
* **Pandas / NumPy**
* **Evaluate (ROUGE, BLEU)**
* **Jupyter Notebook**

---

## 🔧 How It Works

### 1️⃣ Dataset Preparation

* Downloaded Climate TRACE "Top Emission Reduction Strategies" dataset (1,048,576 rows).
* Cleaned and extracted relevant fields:

  * facility name
  * location
  * sector
  * emission reduction potential
  * strategy description
* Created structured `input → output` pairs.

### 2️⃣ Fine-Tuning

* Tokenized dataset using T5 tokenizer
* Trained for 3 epochs
* Achieved excellent ROUGE/BLEU scores
* Saved final model for inference

### 3️⃣ Inference

* Generate strategies for any input facility using:

```python
generate_strategy("Facility: XYZ | Country: USA | Sector: steel | EmissionReductionPotential(Mt): 0.20 | Difficulty: Mid-term")
```

### 4️⃣ Model Comparison

Included notebook demonstrating:

* Base T5 → generic / irrelevant output
* Fine-tuned T5 → precise, actionable, domain-specific recommendations

---

## 📌 Use Cases

* Climate policy analysis
* Decarbonization planning
* Sustainability consulting
* AI for environmental impact reduction
* Industrial emission strategy generation
* Net-Zero transition automation

---

## 🎯 Why This Project Matters

This project shows strong capabilities in:

* **LLM Fine-Tuning**
* **NLP Engineering**
* **Real-World Climate Data Processing**
* **Model Evaluation & Benchmarking**
* **Sustainability + AI intersection**

It is highly relevant for roles in:

* AI/ML Engineering
* NLP Engineer
* Climate AI / Sustainability Tech
* Research Engineer (NLP/LLM)

---

## 🤝 Contributing

Pull requests and suggestions are welcome!
This project aims to be a strong baseline for future sustainability-focused LLM research.

---

## 📬 Contact

**Vipin Tomer**
📧 Email: [tvipin8171@gmail.com](mailto:tvipin8171@gmail.com)
🔗 LinkedIn: [https://www.linkedin.com/in/vipin728/](https://www.linkedin.com/in/vipin728/)
🔗 GitHub: [https://github.com/Vipin8171](https://github.com/Vipin8171)


Just tell me!
