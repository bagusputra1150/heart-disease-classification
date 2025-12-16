# Heart Disease Classification using KNN and Logistic Regression

This repository contains a machine learning project for classifying
heart disease using the Heart Disease dataset. The implementation
is carried out in Python using Google Colab.

The project applies two classification algorithms:
- K-Nearest Neighbor (KNN)
- Logistic Regression

Both models are trained and evaluated using the same preprocessing
pipeline to ensure a fair comparison.

---

## Dataset
The dataset used in this project is the Heart Disease dataset obtained
from Kaggle. The dataset consists of clinical features related to
patients and a target variable indicating the presence of heart disease.

Target variable:
- 0 (Absence): No heart disease
- 1 (Presence): Heart disease

---

## Preprocessing Steps
The following preprocessing steps are performed in the notebook:

1. Loading the dataset using pandas
2. Inspecting data structure and feature names
3. Separating features (X) and target label (y)
4. Splitting the dataset into training and testing sets
   - 80% training data
   - 20% testing data
5. Standardizing feature values using StandardScaler

Standardization is applied because the KNN algorithm is sensitive
to feature scale.

---

## Model Implementation

### K-Nearest Neighbor (KNN)
- Implemented using `KNeighborsClassifier` from scikit-learn
- Uses Euclidean distance to measure similarity
- The value of k is selected based on experimental evaluation
- Prediction is performed based on majority voting of nearest neighbors

### Logistic Regression
- Implemented using `LogisticRegression` from scikit-learn
- Produces probability estimates for each class
- Used as a comparison model against KNN

---

## Model Evaluation
The performance of both models is evaluated using the following metrics:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC Curve and AUC

Confusion matrix analysis is used to examine classification errors,
especially false negatives, which are critical in medical diagnosis.
ROC curves are plotted to evaluate the discriminative capability
of each model.

---

## Results
The experimental results show that both KNN and Logistic Regression
are able to classify heart disease cases with good performance.
The KNN model with an optimal value of k achieved the highest accuracy
on the testing dataset.

---

## Tools and Libraries
- Python
- Google Colab
- pandas
- numpy
- scikit-learn
- matplotlib

---

## How to Run
1. Open the `.ipynb` notebook file using Google Colab.
2. Upload the Heart Disease dataset when prompted.
3. Run all cells sequentially to reproduce the results.

---

## Author
Putra

---

## Notes
This project is developed for academic purposes and serves as a study
case for applying machine learning techniques to medical data.
