# 🧠 AI & ML Internship – Task 5: Decision Trees and Random Forests

## 📌 Objective

The goal of this task is to learn and apply **tree-based models** for classification, compare their performance, interpret their results, and visualize the decision process using **Scikit-learn** and **Graphviz**.

---

## 📂 Dataset

- **Source**: Breast Cancer Wisconsin (Diagnostic) Dataset
- **Target Variable**: `diagnosis` (Malignant = 1, Benign = 0)
- **Features**: 30 numerical features extracted from images of breast masses

---

## 🛠 Tools & Libraries Used

- Python 3.10+
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Graphviz (external tool, used via PATH)

---

## ✅ Steps Performed

### 1. Data Preprocessing
- Loaded the dataset and cleaned irrelevant columns (`id`)
- Encoded the `diagnosis` column (`M` → 1, `B` → 0)
- Split the dataset into **train/test** sets

### 2. Decision Tree Classifier
- Trained a Decision Tree with `max_depth=4` to avoid overfitting
- Visualized the decision tree using both:
  - `matplotlib.pyplot.plot_tree()`
  - `graphviz.Source(export_graphviz(...))`
- Evaluated accuracy and model structure

### 3. Random Forest Classifier
- Trained a **Random Forest** with 100 estimators
- Evaluated model accuracy, confusion matrix, and classification report
- Compared it with the Decision Tree model
- Plotted **feature importances** using a bar chart

### 4. Overfitting Analysis
- Controlled `max_depth` in Decision Tree to avoid overfitting
- Noted that Random Forest reduces overfitting using **bagging** and ensemble learning

### 5. Cross-Validation (Optional)
- Can use `cross_val_score()` for better model evaluation

---

## 📈 Results

| Model             | Accuracy |
|------------------|----------|
| Decision Tree     | ~92%     |
| Random Forest     | ~96%     |

---

## 📊 Feature Importance

Top features used by the Random Forest model:

---

## 🌳 Decision Tree Visualization

> The decision tree was saved as a `.png` file using `Graphviz` and automatically opened via Python.

If you're using this locally:
- Make sure to install Graphviz and add its `/bin` folder to your system `PATH`.

---

## 🧪 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/Rohith0750/Elevatelabs

   cd your-Eelvate-labs


Run the notebook or script:

task5_decision_tree_random_forest.ipynb

or main.py

# 📁 Files Included
task5_decision_tree_random_forest.ipynb – Full working notebook

decision_tree.png – Tree visualization

README.md – This file

requirements.txt – List of dependencies

dataset.csv – Breast cancer dataset (or link to source)

# ❓ Interview Questions Covered
How does a decision tree work?

What is entropy and information gain?

What is overfitting and how to prevent it?

How is Random Forest better than a single tree?

What is bagging?

How to interpret feature importance?

Pros and cons of decision trees and Random Forests?

🔗 Submission
GitHub Repo: [Your Repository Link Here]

Submitted via internship portal ✅

🙌 Credits
Scikit-learn

UCI ML Repository – Breast Cancer Dataset

markdown
Copy code

---

### ✅ What to Do Next

1. Save this content as `README.md` in your repo.
2. Add other required files:
   - `task5_decision_tree_random_forest.ipynb`
   - `decision_tree.png`
   - `requirements.txt` (let me know if you need help generating this)
3. Push everything to GitHub.
4. Submit the link using the portal.

Let me know if you want the `requirements.txt` or `.ipynb` template as well.
