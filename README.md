  ## Data Mining and Machine Learning 

## Project Title
Heart Disease Classification Using Machine Learning Models


## Project Description

This project aims to develop and evaluate a complete machine learning workflow for predicting heart disease status using a real-world dataset.

The project includes the following steps:

- Dataset understanding and exploration
- Data preprocessing
- Handling missing values
- Encoding categorical variables
- Feature scaling
- Principal Component Analysis (PCA)
- Training multiple classification models
- Cross-validation
- Performance evaluation
- Comparative analysis and model selection

The following classification algorithms were implemented:

- Logistic Regression
- Decision Tree Classifier
- Support Vector Machine (SVM)


The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix


---

# Dataset

Dataset Name:
Heart Disease Dataset

Dataset Source:
https://www.kaggle.com/datasets/oktayrdeki/heart-disease

Number of Samples:
10000 samples

Number of Input Features:
20 features

Target Variable:

Heart Disease Status

Target Encoding:

- No → 0
- Yes → 1


---

# Project Files Structure


DMML_Assignment/
│
├── assignment.ipynb
├── heart_disease.csv
├── README.md


---

# Requirements

The project requires Python 3 and the following libraries:

- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn


Install the required libraries using:


pip install pandas numpy scikit-learn matplotlib seaborn


---

# How to Run the Project

## Method 1: Using Jupyter Notebook

1. Install Jupyter Notebook if it is not installed:


pip install notebook


2. Open Command Prompt or Terminal.

3. Navigate to the project folder:


cd path_to_project_folder


4. Start Jupyter Notebook:


jupyter notebook


5. A browser window will open. Open the file:


DMML_Assignment.ipynb


6. Run the notebook cells sequentially from Task 1 to Task 8.


---

## Method 2: Using Visual Studio Code

1. Install Visual Studio Code.

2. Install the following extensions:
   
   - Python Extension
   - Jupyter Extension

3. Open Visual Studio Code.

4. Select:


File → Open Folder


and choose the project folder.

5. Open the notebook file:


DMML_Assignment.ipynb


6. Select the Python interpreter:


Kernel → Select Kernel → Python Environment


7. Run the cells sequentially using:


Run Cell


or:


Shift + Enter



---

# Data Preprocessing

The following preprocessing techniques were applied:

- Duplicate records checking
- Missing value handling:
  - Median imputation for numerical features
  - Most frequent value imputation for categorical features
- Target variable encoding
- One-Hot Encoding for categorical variables
- StandardScaler for numerical features


After preprocessing:

- Original features: 20 features
- Processed features after encoding: 35 features


---

# Principal Component Analysis (PCA)

PCA was applied after feature scaling to reduce dimensionality while preserving important information.

The obtained dimensions were:

- Original processed features: 35 features
- PCA preserving 90% variance: 20 components
- PCA preserving 95% variance: 22 components


---

# Machine Learning Models

The following models were trained using:

- Original processed features
- PCA 90% transformed features
- PCA 95% transformed features


Implemented models:

1. Logistic Regression
2. Decision Tree Classifier
3. Support Vector Machine (SVM)


---

# Final Model Selection

Based on the evaluation results, the selected model was:

**SVM using PCA 95% features**

The model was selected because it achieved the best balance between Recall and F1-score, which are important metrics for medical classification problems with imbalanced classes.

Although Decision Tree achieved higher accuracy, it showed a low ability to detect positive heart disease cases. Therefore, SVM PCA 95% was considered more suitable for identifying heart disease cases.


---

# Authors

Student 1:
Hamsa Hantash

Student 2:
Ghada Qnazea
