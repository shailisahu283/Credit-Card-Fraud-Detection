# 💳 Credit Card Fraud Detection using Machine Learning

![fraud-banner](https://user-images.githubusercontent.com/your-image-url/fraud-banner.png) <!-- (Optional visual banner) -->

---

## 📌 Project Objective

The aim of this project is to detect **fraudulent credit card transactions** using various Machine Learning algorithms on a highly imbalanced dataset.  
We compare models ranging from simple Logistic Regression to advanced ensemble methods like **XGBoost** and **LightGBM**.

---

## 🔍 Dataset Summary

- Source: [Kaggle - Fraud Detection Dataset](https://www.kaggle.com/datasets/kartik2112/fraud-detection)
- Total Records: `555,719`
- Target Variable: `is_fraud` (`1 = Fraud`, `0 = Genuine`)
- Imbalance: Only ~0.3% transactions are fraud

---

## 🔧 How to Run the Project

> Run the notebook in **Google Colab**(https://colab.research.google.com/drive/177deY5TrjroqM1v6xi7T5QDdN99_jYav?usp=sharing) or any Jupyter environment.

### 🛠️ Prerequisites

```bash
pip install kagglehub xgboost lightgbm seaborn scikit-learn
```

### 📁 Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/fraud-detection-ml.git
   cd fraud-detection-ml
   ```

2. Run `main.ipynb` or `fraud_detection.ipynb` for full workflow:
   - Data loading and exploration
   - Feature engineering
   - Model training (Logistic Regression, Random Forest, XGBoost, LightGBM)
   - Performance metrics and plots

---

## 🔬 Models & Results

| Model               | Precision (Fraud) | Recall (Fraud) | ROC AUC |
|--------------------|-------------------|----------------|---------|
| Logistic Regression| 0.02              | 0.78           | 0.89    |
| Random Forest       | 0.83              | 0.34           | 0.92    |
| XGBoost             | 0.39              | 0.65           | 0.97    |
| LightGBM            | 0.06              | 0.87           | 0.97    |

> 📌 **Observation:** Boosting models (XGBoost & LightGBM) handled imbalance far better due to their ability to focus on hard examples.

---

## 🧠 Key Takeaways

- Data was highly imbalanced, requiring careful metric selection (ROC AUC, Recall).
- Categorical encoding (merchant, gender, state, day) was important for model performance.
- Ensemble methods (Random Forest, XGBoost, LightGBM) significantly outperformed linear models.

---

## 📎 Repository Structure

```
📁 fraud-detection-ml
│
├── 📄 README.md                <- You are here
├── 📄 requirements.txt         <- Python dependencies
├── 📒 fraud_detection.ipynb    <- Main analysis notebook
├── 📁 /plots                   <- Saved plots (optional)
└── 📁 /data                    <- Loaded via kagglehub
```

---

## 🤝 Acknowledgements

- Dataset: [Kaggle - Kartik2112](https://www.kaggle.com/datasets/kartik2112/fraud-detection)
- Libraries: `sklearn`, `xgboost`, `lightgbm`, `seaborn`, `pandas`, `matplotlib`

---

## 🧑‍💻 Author

Made with ❤️ by Shaili Sahu(https://github.com/shailisahu283)

```
