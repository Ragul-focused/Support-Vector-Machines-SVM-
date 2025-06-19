# 🧪 Breast Cancer Classification with Support Vector Machines (SVM)

This project is part of the **AI & ML Internship - Task 7**. It focuses on implementing Support Vector Machines for binary classification using the **Breast Cancer Wisconsin dataset**. We explore both **linear** and **non-linear (RBF kernel)** SVMs, along with hyperparameter tuning and visualization of decision boundaries.

---

## 🎯 Objective

- Train and evaluate SVM classifiers with different kernels
- Understand the role of `C`, `gamma`, and kernel functions
- Visualize decision boundaries in reduced 2D feature space
- Perform model tuning using `GridSearchCV` and cross-validation

---

## 📁 Dataset

- **Source:** [Breast Cancer Wisconsin Dataset (Kaggle)](https://www.kaggle.com/datasets/yasserh/breast-cancer-dataset)
- **Samples:** 569
- **Features:** 30 numerical measurements from digitized images of breast mass
- **Target:** Diagnosis — Malignant (1) or Benign (0)

---

## 🛠 Tools & Libraries

- **Python**
- **Scikit-learn** – SVM, metrics, scaling, PCA
- **Pandas, NumPy** – Data handling
- **Matplotlib, Seaborn** – Visualization

---

## 🧪 Steps Performed

### 1. Data Preparation
- Loaded the breast cancer dataset
- Scaled features using `StandardScaler`

### 2. Model Training
- Trained two SVM classifiers:
  - **Linear SVM** (`kernel='linear'`)
  - **RBF SVM** (`kernel='rbf'`, with `C` and `gamma` tuning)

### 3. Evaluation
- Evaluated using:
  - Accuracy
  - Confusion matrix
  - Classification report

### 4. Hyperparameter Tuning
- Used `GridSearchCV` to find best `C` and `gamma`
- 5-fold cross-validation

### 5. Visualization (Optional)
- Reduced features to 2D using PCA
- Plotted decision boundaries

---

## 📊 Results

| Model        | Accuracy | Best Parameters (if tuned)       |
|--------------|----------|----------------------------------|
| Linear SVM   | 96.5%    | `kernel='linear'`                |
| RBF SVM      | 98.2%    | `C=10`, `gamma=0.01`, `kernel=rbf` |

> 🔍 The RBF kernel achieved better performance due to its flexibility in modeling non-linear boundaries.

---

## 📈 Visuals

### 🎯 Confusion Matrix (RBF SVM)

![Screenshot 2025-06-19 172352](https://github.com/user-attachments/assets/ca2673c6-a4c1-4cee-bcd1-a416b6754669)


### 🌀 Decision Boundary in 2D (PCA + SVM)

![Screenshot 2025-06-19 172111](https://github.com/user-attachments/assets/0f6637bd-7d58-44d4-a674-d2b3879dda44)


---



