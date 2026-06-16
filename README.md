<div align="center">

# 🚢 Titanic Survival Prediction

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)](https://matplotlib.org)

> **Can we predict who survived the Titanic disaster using passenger data?**
> A complete supervised ML pipeline — from raw data to actionable insights.

</div>

---

## 📌 Problem Statement

On April 15, 1912, the RMS Titanic sank after colliding with an iceberg, killing 1,502 out of 2,224 passengers. This project uses passenger data (age, gender, ticket class, family size) to **predict survival outcomes** using Logistic Regression — and uncovers the hidden patterns that determined who lived and who didn't.

---

## 🎯 Project Highlights

| What | Detail |
|------|--------|
| 🧠 Algorithm | Logistic Regression (Classification) |
| 📦 Dataset | Titanic dataset — 891 passengers, 12 features |
| 🎯 Target | Survived (0 = No, 1 = Yes) |
| 📊 Key Features | Age, Sex, Pclass, Fare, SibSp, Parch, Embarked |
| ✅ Accuracy | ~80% on test set |

---

## 🗂️ Project Structure

```
titanic-survival-prediction/
│
├── titanic_survival_prediction.ipynb  # Jupyter Notebook — full ML pipeline with outputs
├── train.csv                          # Training dataset
├── requirements.txt                   # Dependencies
├── images/                            # Visualization outputs
└── README.md
```

---

## 🔄 ML Pipeline

```
Raw Data  →  Data Cleaning  →  Feature Engineering  →  Model Training  →  Evaluation  →  Insights
```

**Step-by-step:**

1. **Load Data** — Read `train.csv` using Pandas
2. **Handle Missing Values** — Fill `Age` with median, `Embarked` with mode
3. **Encode Categoricals** — Label encode `Sex` and `Embarked`
4. **Feature Selection** — Use `Age`, `Fare`, `Pclass`, `Sex`, `SibSp`, `Parch`
5. **Train/Test Split** — 80/20 split using `train_test_split`
6. **Train Model** — Logistic Regression via Scikit-learn
7. **Evaluate** — Accuracy, Precision, Recall, F1-Score

---

## 📊 Key Findings

- 👩 **Women survived at ~74%** vs men at ~19% — gender was the strongest predictor
- 🎟️ **1st class passengers** had 3x higher survival rate than 3rd class
- 👶 **Children (< 10 years)** had significantly higher survival rates
- 💰 **Higher fare** correlated strongly with survival (proxy for wealth/class)

---

## 📈 Visualizations

> Charts are saved in the `images/` folder after running the script.

- Survival rate by **Gender**
- Survival rate by **Passenger Class**
- Survival distribution by **Age Group**
- **Correlation heatmap** of features

---

## ⚙️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/keerthanad29/titanic-survival-prediction.git
cd titanic-survival-prediction

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter Notebook
jupyter notebook titanic_survival_prediction.ipynb
```

> Or open directly in **Google Colab** — no setup needed!

---

## 📦 Requirements

```
pandas
numpy
scikit-learn
matplotlib
seaborn
```

---

## 🧠 Model Performance

| Metric | Score |
|--------|-------|
| Accuracy | ~80% |
| Precision | ~78% |
| Recall | ~74% |
| F1-Score | ~76% |

---

## 💡 What I Learned

- End-to-end ML workflow: data cleaning → feature engineering → model evaluation
- Importance of **handling missing data** correctly (median vs mean vs mode)
- How **label encoding** works for categorical variables
- Interpreting **classification metrics** beyond just accuracy

---

## 🔮 Future Improvements

- [ ] Try Random Forest / XGBoost for better accuracy
- [ ] Add cross-validation
- [ ] Build an interactive prediction web app using Streamlit
- [ ] Perform hyperparameter tuning with GridSearchCV

---
