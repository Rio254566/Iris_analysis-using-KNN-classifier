#  Iris Flower Classification using K-Nearest Neighbors (KNN)

This project explores the famous **Iris dataset** and applies the **K-Nearest Neighbors (KNN)** classification algorithm to classify iris flowers into three species: *Setosa*, *Versicolor*, and *Virginica*. The project includes thorough **data preprocessing**, **visualization**, **model training**, and **evaluation**.

---

##  Project Structure

- **Dataset**: Built-in `sklearn.datasets.load_iris()` dataset
- **Models**: K-Nearest Neighbors Classifier
- **Preprocessing**: Outlier removal, normalization
- **Evaluation**: Accuracy, confusion matrix, classification report
- **Visualization**: 2D decision boundaries, 3D & 4D data plots

---

##  Tasks Completed

### 1.  Exploratory Data Analysis (EDA)
- Loaded the dataset and converted it to a `pandas DataFrame`.
- Displayed dataset shape, class distribution, and feature info.
- Used **boxplots** and **pairplots** to visualize feature distributions and identify outliers.

### 2.  Data Preprocessing
- **Missing Value Check**: Confirmed there were no missing values.
- **Outlier Removal**:
  - Used boxplots to detect outliers in numeric features.
  - Removed extreme outliers to improve model performance.
- **Feature Scaling**:
  - Applied **z-score normalization** (`StandardScaler`) to standardize features.

### 3.  Model Training with KNN
- Split data into **training and test sets** using `train_test_split`.
- Trained `KNeighborsClassifier` on the training data.
- Experimented with different values of **k** (number of neighbors) to evaluate performance.

### 4.  Model Evaluation
- Evaluated using:
  -  **Accuracy Score**
  -  **Confusion Matrix**
  -  **Classification Report** (Precision, Recall, F1-Score)
- Selected the best `k` value based on accuracy.

### 5.  Visualizations
- **2D Decision Boundary**:
  - Plotted decision regions using first two features to visualize how KNN classifies.
- **3D Scatter Plot**:
  - Visualized the first 3 features in a 3D space, colored by class.
---

##  Model Summary

| k Value | Accuracy |
|---------|----------|
| 1       | 96.67%   |
| 3       | 100.00%  |
| 5       | 100.00%  |

** KNN performed **very well** on the Iris dataset with **k = 3 or 5**, giving perfect classification on the test set.

---

## 🔧 Requirements

```bash
pip install pandas scikit-learn matplotlib seaborn
