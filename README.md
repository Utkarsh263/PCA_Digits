# 📊 PCA Dimensionality Reduction & Classification Project

## 🔷 Project Overview

This project demonstrates the use of **Principal Component Analysis (PCA)** for dimensionality reduction and evaluates its impact on classification performance using Logistic Regression. The goal is to reduce the number of features while preserving maximum information and maintaining high model accuracy.

Dimensionality reduction helps improve model efficiency, reduce computation time, and remove redundant features while retaining important variance in the dataset.

---

## 🔷 Dataset Used

**Primary Dataset:** Sklearn Digits Dataset

* Contains handwritten digit images (0–9)
* Total Samples: 1797
* Features per image: 64 (8×8 pixel images flattened)
* Target: Digit label (0–9)

---

## 🔷 Technologies & Libraries

* Python
* NumPy
* Matplotlib
* Scikit-learn
* PCA (Principal Component Analysis)
* Logistic Regression

---

## 🔷 Project Workflow

### 1. Data Loading

Loaded handwritten digits dataset from sklearn and separated features and labels.

### 2. Data Preprocessing

* Flattened image dataset already provided in tabular format
* Applied **StandardScaler** for feature scaling
* Scaling ensures PCA performs correctly since it is variance-based

### 3. Train-Test Split

Split dataset into:

* 80% training data
* 20% testing data

Used for unbiased model evaluation.

### 4. Model Training (Original Dataset)

Trained Logistic Regression on original 64-feature dataset.
Evaluated baseline accuracy for comparison.

### 5. PCA Dimensionality Reduction

Applied PCA with multiple component values:

* 2 components
* 10 components
* 30 components
* 50 components

Reduced feature space while preserving maximum variance.

### 6. Model Training on Reduced Data

Trained Logistic Regression again on PCA-transformed dataset.
Compared accuracy with original dataset.

### 7. Explained Variance Analysis

Generated cumulative explained variance plot to determine optimal number of components required to retain ~95% information.

### 8. Data Visualization

Used PCA (2 components) to visualize digit clusters in 2D space.
Observed separation between digit classes after dimensionality reduction.

---

## 🔷 Results & Observations

* PCA significantly reduced number of features from 64 to optimal components
* Around 30 components retained most of the variance (~95%)
* Logistic Regression achieved nearly same accuracy on reduced dataset
* Reduced dimensionality improved computational efficiency
* 2D PCA visualization showed clear clustering of digit classes

---

## 🔷 Key Learnings

* PCA helps remove redundant and correlated features
* Feature scaling is essential before applying PCA
* Explained variance helps choose optimal components
* Dimensionality reduction can maintain performance while reducing complexity
* Visualization using PCA helps understand data separation

---

## 🔷 Conclusion

This project demonstrates how PCA can effectively reduce feature dimensions while maintaining classification accuracy. It highlights the trade-off between dimensionality reduction and model performance and shows how optimal component selection improves efficiency without significant accuracy loss.

---

## 🔷 Future Improvements

* Apply PCA on MNIST dataset (70,000 images)
* Compare with other models like SVM and KNN
* Hyperparameter tuning for improved accuracy
* Deploy model using Streamlit
* Use t-SNE for advanced visualization

---

## 🔷 Author

**Utkarsh Kohli**

