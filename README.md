# Cancer Prognostic Outcome Classification Using TCGA RNA-Seq Profiles 🧬

This project applies **bioinformatics and machine learning** methods to RNA-Seq data from **The Cancer Genome Atlas (TCGA)** to explore whether gene expression patterns can help classify cancer patients into good vs. poor prognostic groups.

---

## 📂 Contents
- 📓 [CancerDataAnalysis.ipynb](CancerDataAnalysis.ipynb)
---

## 🔍 Methods
- **Differential Expression Analysis**: t-tests with Benjamini–Hochberg correction identified ~7,800 significant genes
- **Feature Selection**: top 100 genes with strongest signal carried forward  
- **Unsupervised Learning**: k-means clustering and t-SNE revealed prognosis-enriched patient clusters
- **Classification Models**:  
  - Logistic Regression (L1 regularised)  
  - Gradient Boosted Trees  
  - Achieved AUC ≈ 0.69 on hold-out set 
- **Gene Ontology Enrichment**: highlighted proteasome, DNA replication, and mitotic cell cycle pathways

---

## 📊 Key Results
- Even with modest fold-changes, clustering on a 100-gene signature showed **statistically significant separation** of outcomes (χ² p < 1e-16).  
- Baseline classifiers showed **moderate discriminative power** (AUC ~0.69 hold-out).  
- GO terms confirmed known hallmarks of aggressive tumours (DNA repair, mitotic cycle, proteasome activity).  

---

## 🛠️ Tech Stack
- Python (Google Colab)  
- pandas, scikit-learn, seaborn, gseapy  
- Dataset: The Cancer Genome Atlas (TCGA) Pan-Cancer RNA-Seq profiles The Cancer Genome Atlas 

---

## 👥 Credits
Developed by **Mahya Mottaghi** as part of *CS 4973 / 5483 Bio Data Science (Spring 2025)*.  

---
