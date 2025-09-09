# Alzheimer’s Blood Transcriptomic ML Pipeline 🧬🧠  
*A journey into blood transcriptomics and machine learning for Alzheimer’s*  

---

## Why I built this
Alzheimer’s is one of the toughest health challenges of our time.  
I was curious: **can we detect Alzheimer’s just from a person’s blood gene expression?**  

So I took a real dataset from the Gene Expression Omnibus (**GSE63060** on platform **GPL6947**),  
and built a full machine learning pipeline — from raw probes to an interpretable **20-gene signature**.  

---

## What I did
- Downloaded and parsed GEO data (expression + metadata).  
- Mapped **Illumina probes → gene symbols**.  
- Compared **baseline logistic regression** vs **XGBoost**.  
- Used **SHAP** to find the most important probes.  
- Distilled it down to a compact **20-gene logistic regression model**.  
- Validated with **5-fold cross-validation**, making sure feature selection stayed **inside each fold** (to avoid leakage).  

---
## Results 
Here’s how the models performed (on held-out test set):  

| Model | ROC AUC | PR AUC |
|------:|:-------:|:------:|
| Logistic Regression (all features) | *fill in* | *fill in* |
| XGBoost | *fill in* | *fill in* |
| **20-gene Logistic Regression** | **fill in** | **fill in** |
