# 🏡 California House Price Prediction
### Feature Engineering · Model Optimization · Performance Comparison

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-orange?logo=scikit-learn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

---

## 📌 Project Overview

This project is part of the **Maincrafts Technology AI/ML Internship – Task 2**.  
It demonstrates how Machine Learning engineers improve models in real-world projects by applying **feature scaling**, training **multiple regression algorithms**, and selecting the best performer using measurable metrics.

> **Task 1** covered basic model training. **Task 2** goes further — this is where professional ML practice begins.

---

## 🎯 Objectives

- Prepare and scale data correctly for Machine Learning
- Train and compare multiple regression models
- Evaluate models using RMSE and R² Score
- Select and justify the best-performing model
- Follow an industry-aligned ML pipeline

---

## 📊 Results at a Glance

| Model | RMSE ↓ | R² Score ↑ | Verdict |
|---|---|---|---|
| Linear Regression | 0.4241 | 0.8374 | Baseline |
| Ridge Regression | 0.4241 | 0.8374 | Similar to LR |
| **Decision Tree (depth=5)** | **0.3122** | **0.9119** | ✅ Best Model |

**Winner: Decision Tree Regressor** — 91.2% variance explained, lowest prediction error.


---

## 🗂️ Repository Structure

```
ml-house-price-prediction/
│
├── notebooks/
│   └── AI_ML_Task2_Model_Comparison.ipynb   # Full step-by-step implementation
│
├── reports/
│   └── AI_ML_Task2_Report.pdf               # 2-page professional report
│
├── models/
│   └── best_model.pkl                       # Saved Decision Tree (joblib)
│
├── assets/
│   ├── performance_plot.png                 # Actual vs Predicted + R² chart
│   └── rmse_plot.png                        # RMSE comparison chart
│
└── README.md
```

---

## 🧰 Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.12 | Core language |
| pandas / NumPy | Data manipulation |
| scikit-learn | ML models & preprocessing |
| matplotlib | Visualisation |
| joblib | Model serialisation |
| Jupyter Notebook | Interactive development |

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/ml-house-price-prediction.git
cd ml-house-price-prediction
```

### 2. Install dependencies
```bash
pip install pandas numpy scikit-learn matplotlib joblib jupyter
```

### 3. Run the notebook
```bash
jupyter notebook notebooks/AI_ML_Task2_Model_Comparison.ipynb
```

### 4. Load the saved model
```python
import joblib
model = joblib.load('models/best_model.pkl')
predictions = model.predict(X_test_scaled)
```

---

## 📋 Step-by-Step Pipeline

```
1. Import Libraries
2. Load Dataset          → California Housing (20,640 samples)
3. Separate X and y      → Features vs Target
4. Feature Scaling       → StandardScaler (mean=0, std=1)
5. Train-Test Split      → 80% train / 20% test
6. Train Models          → Linear, Ridge, Decision Tree
7. Evaluate Models       → RMSE + R² on test set
8. Visual Validation     → Actual vs Predicted scatter + bar charts
9. Save Best Model       → joblib serialisation
```

---

## 💡 Key Concepts Learned

- **Feature Scaling** — prevents large-range features from dominating learning
- **Model Comparison** — never rely on a single algorithm; always benchmark
- **Evaluation Metrics** — RMSE measures error magnitude; R² measures explanatory power
- **Overfitting Prevention** — max_depth=5 on Decision Tree avoids memorising training data
- **ML Workflow** — mirrors real industry practices end-to-end

---

## 📄 Report

A detailed 2-page PDF report is available in [`reports/AI_ML_Task2_Report.pdf`](reports/AI_ML_Task2_Report.pdf) covering methodology, results, charts, and model selection justification.

---

## 🤝 Acknowledgements

Built as part of the **Maincrafts Technology AI/ML Internship Program**.  
Dataset: [California Housing Dataset](https://scikit-learn.org/stable/datasets/real_world.html) via scikit-learn.

---

## 📬 Contact

Feel free to connect or raise an issue if you have questions!

⭐ If this project helped you, give it a star!
