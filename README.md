# 🧠 Support Vector Machines (SVM) for Classification

## 📌 Objective
Use Support Vector Machines (SVMs) to perform **linear and non-linear classification** on the Breast Cancer dataset, visualize decision boundaries, tune hyperparameters, and evaluate model performance.

---

## 🛠️ Tools & Libraries
- **Scikit-learn** → Model training, preprocessing, evaluation
- **NumPy** → Numerical computations
- **Matplotlib** → Visualization

---

## 📂 Dataset
We use the **Breast Cancer dataset**, which contains features of cell nuclei from breast mass images.  
The target variable is **`diagnosis`**:
- `M` = Malignant (1)  
- `B` = Benign (0)  

Columns include:
['id', 'diagnosis', 'radius_mean', 'texture_mean', 'perimeter_mean',
'area_mean', 'smoothness_mean', 'compactness_mean', 'concavity_mean',
'concave points_mean', 'symmetry_mean', 'fractal_dimension_mean', ...]


We drop the `id` column and select two features (`radius_mean`, `texture_mean`) for visualization.

---

## 🚀 Steps

### 1. Load & Preprocess Data
- Drop irrelevant columns (`id`).
- Encode target (`M` → 1, `B` → 0).
- Train-test split (80-20).
- Standardize features.

### 2. Train SVM Models
- **Linear Kernel** (`kernel='linear'`)
- **RBF Kernel** (`kernel='rbf'`)

### 3. Visualize Decision Boundaries
- Plot decision boundaries with contour plots.
- Highlight support vectors.

### 4. Hyperparameter Tuning
- Tune **C** and **gamma** using `GridSearchCV`.

### 5. Cross-Validation
- Evaluate model using 5-fold CV accuracy.

---

## 📊 Results
- Linear SVM works when classes are linearly separable.
- RBF kernel captures **non-linear** relationships.
- Hyperparameter tuning (C, gamma) improves accuracy.
- Cross-validation helps check **generalization performance**.

---

## 🖼️ Visualizations
- Decision boundary plots for **Linear** and **RBF kernels**.
- Cross-validation accuracy results.

---

## 📌 References
- [Scikit-learn SVM Documentation](https://scikit-learn.org/stable/modules/svm.html)
- [Breast Cancer Dataset](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29)

---
