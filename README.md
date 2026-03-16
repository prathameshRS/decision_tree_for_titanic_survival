# 🌳 Decision Tree — Titanic Survival Prediction

A machine learning project that predicts whether a passenger
survived the Titanic disaster using a Decision Tree Classifier.

---

## 📌 About the Project

This project uses the famous Titanic dataset to build a
Decision Tree model that predicts survival based on
passenger details like age, gender, ticket class, and fare.

---

## 📊 Dataset

- **Source:** [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic)
- **Total Passengers:** 891
- **Features:** 7
- **Target:** Survived (1) or Died (0)

---

## 🔑 Features Used

| Feature | Description |
|---|---|
| Pclass | Ticket class (1, 2, 3) |
| Sex | Gender (0=male, 1=female) |
| Age | Age of passenger |
| SibSp | Number of siblings/spouses |
| Parch | Number of parents/children |
| Fare | Ticket fare |
| Embarked | Port of embarkation |

---

## ⚙️ Steps Followed
```
1. Loaded Titanic dataset
2. Handled missing values
   → Age     → filled with mean
   → Embarked → filled with mode
   → Cabin   → dropped (too many missing)
3. Dropped useless columns (Name, Ticket, PassengerId)
4. Converted text to numbers (Sex, Embarked)
5. Split data → 80% train, 20% test
6. Trained Decision Tree (max_depth=4)
7. Evaluated accuracy
8. Visualized the tree
9. Predicted new passengers
```

---

## 📈 Model Performance

| Metric | Score |
|---|---|
| Accuracy | 74% |
| Algorithm | CART |
| Max Depth | 3 |

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

---

## 🚀 How to Run

### Step 1 — Clone the repo
```bash
git clone https://github.com/yourusername/decision-tree-titanic
```

### Step 2 — Install libraries
```bash
pip install scikit-learn pandas matplotlib numpy
```

### Step 3 — Run the notebook
```bash
jupyter notebook decision_tree_titanic.ipynb
```

---

## 📂 Project Structure
```
decision-tree-titanic/
│
├── train.csv                       ← dataset
├── decision_tree_titanic.ipynb     ← main notebook
└── README.md                       ← this file
```

---

## 🧠 What I Learned

- How Decision Tree algorithm works
- CART algorithm and Gini Impurity
- Handling missing values
- Converting text to numbers
- Controlling overfitting with max_depth
- Visualizing a Decision Tree

---

## 📊 Decision Tree Visualization

The tree asks questions like:
```
Is passenger female?
    ├── YES → likely Survived ✅
    └── NO  → Is class = 1st?
                  ├── YES → likely Survived ✅
                  └── NO  → likely Died ❌
```

---

## 🔮 Sample Predictions

| Pclass | Sex | Age | Result |
|---|---|---|---|
| 3 | Male | 22 | Died ❌ |
| 1 | Female | 25 | Survived ✅ |

---

## 👤 Author

**prathamesh sahastrabuddhe**
- GitHub: https://github.com/prathameshRS
- LinkedIn: https://www.linkedin.com/in/prathamesh-sahastrabuddhe2003/
- Medium: https://medium.com/@prathameshsahastrabuddhe2003
