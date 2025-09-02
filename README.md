# Introduction to Machine Learning — Final Project (TAU, Spring 2023)

A compact, end‑to‑end **supervised learning** project focused on building and evaluating multiple classifiers on a tabular dataset.  
The notebook walks through **EDA → preprocessing → modeling → evaluation → test-time inference**, with clear, reproducible steps and extensive comments.

---

## Highlights
- 📊 **Exploratory Data Analysis (EDA):** data overview, distributions, correlation inspection, and feature behavior checks.
- 🧼 **Preprocessing Pipeline:** missing values, outlier handling, categorical/binary encoding, scaling, and optional **PCA** for dimensionality reduction.
- 🤖 **Models Compared:** Logistic Regression, Random Forest, Multi‑Layer Perceptron (MLP), and **SVM** (with RBF grid search).
- ✅ **Evaluation:** K‑Fold cross‑validation, ROC curves/AUC and confusion matrices; train vs. validation curves to check over/under‑fitting.
- 🚀 **Reproducibility:** deterministic splits and a single notebook you can run end‑to‑end.

---

## Repository Structure
```
.
├── Project.ipynb        # Main end-to-end workflow (EDA → Preprocess → Train → Evaluate → Test)
├── .gitignore
└── README.md
```

---

## Methodology (What You'll See in the Notebook)

1. **EDA**
   - Data shape, types
   - Numeric summaries and visual checks (distributions, potential outliers)
   - Categorical feature review

2. **Preprocessing**
   - Missing value imputation
   - Outlier treatment
   - Encoding of categorical and binary features (ordinal vs. non‑ordinal)
   - Feature scaling (**MinMaxScaler**)
   - Optional **PCA** for dimensionality control

3. **Modeling**
   - **Logistic Regression** baseline
   - **Random Forest** with tuned depth, leaf sizes, and trees
   - **MLP** (hidden layers, learning rate, batch size)
   - **SVM (RBF)** with `C`/`gamma` search

4. **Evaluation**
   - **K‑Fold cross‑validation**
   - **ROC curves** and **AUC**
   - **Confusion matrices**
   - Train vs. validation learning curves

5. **Final Selection & Test Inference**
   - Refit the chosen model on the full training set
   - Predict on `test.csv` and export results

---

## What I Focused On
- **Clarity:** Every step is explained inline; variable names are explicit.
- **Rigor:** Multiple strong baselines and tuned models; *guardrails* against data leakage.
- **Maintainability:** Modular cell structure and a predictable folder layout.
- **Communication:** Visuals + metrics to explain trade‑offs, not just a single score.

---

## Tech Stack
- Python, NumPy, Pandas, Matplotlib, Seaborn
- scikit‑learn, SciPy

---

## Author
**Tzlil Boostani** — Industrial Engineering & Management