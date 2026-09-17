# AI Insurance Purchase Prediction

## 📌 Project Overview

This project uses **Machine Learning classification algorithms** to predict whether a customer is likely to purchase insurance based on their:

* **Age**
* **Estimated Salary**

The project compares multiple classification algorithms and evaluates their performance using accuracy, precision, recall, F1-score, and confusion matrices.

---

## 🎯 Problem Statement

The objective is to develop an AI-based classification system that predicts whether a customer will purchase insurance.

The project also compares different Machine Learning algorithms to understand their performance and generalization ability.

### Input

* Customer Age
* Customer Estimated Salary

### Output

* `0` → Customer is predicted **not to purchase**
* `1` → Customer is predicted **to purchase**

---

## 🎯 Objectives

The main objectives of this project are:

1. Analyze the relationship between age, salary, and insurance purchase.
2. Preprocess the dataset for Machine Learning.
3. Train multiple classification algorithms.
4. Compare the performance of the algorithms.
5. Predict insurance purchase for different customer profiles.
6. Analyze different age and salary scenarios.
7. Test hypotheses related to age and salary.
8. Identify useful patterns in customer behavior.

---

## 📊 Dataset

The project uses the **Social Network Ads dataset**.

### Dataset File

```text
Social_Network_Ads.csv
```

### Important Columns

| Column          | Description                                |
| --------------- | ------------------------------------------ |
| Age             | Customer's age                             |
| EstimatedSalary | Customer's estimated salary                |
| Purchased       | Whether the customer purchased the product |

### Target Variable

```text
Purchased
```

Values:

```text
0 = No Purchase
1 = Purchase
```

---

## 🤖 Machine Learning Algorithms

Five classification algorithms are implemented:

### 1. Logistic Regression

Logistic Regression is used for binary classification problems.

It predicts the probability of a customer purchasing insurance.

---

### 2. K-Nearest Neighbors (KNN)

KNN predicts the class of a customer based on nearby data points.

In this project:

```text
n_neighbors = 5
```

---

### 3. Support Vector Machine (SVM)

SVM finds a decision boundary that separates customers into different classes.

The project uses an RBF kernel.

---

### 4. Decision Tree

Decision Tree creates a tree-like structure of decisions based on customer features.

The project uses:

```text
criterion = entropy
```

---

### 5. Random Forest

Random Forest combines multiple decision trees to make predictions.

The project uses:

```text
n_estimators = 100
```

---

## ⚙️ Methodology

The project follows these steps:

```text
Dataset
   ↓
Data Cleaning
   ↓
Feature Selection
   ↓
Train-Test Split
   ↓
Feature Scaling
   ↓
Machine Learning Models
   ↓
Predictions
   ↓
Performance Evaluation
   ↓
Model Comparison
   ↓
Customer Prediction
   ↓
Hypothesis Analysis
```

---

## 🔧 Data Preprocessing

The following preprocessing steps are performed:

1. Load the dataset.
2. Check dataset dimensions.
3. Check missing values.
4. Select `Age` and `EstimatedSalary` as input features.
5. Select `Purchased` as the target variable.
6. Split the dataset into training and testing sets.
7. Apply StandardScaler to scale the features.

### Train-Test Split

```text
Training Data = 75%
Testing Data = 25%
```

---

## 📏 Evaluation Metrics

The models are evaluated using:

### Accuracy

Measures the percentage of correct predictions.

### Precision

Measures how many predicted purchases were actually purchases.

### Recall

Measures how many actual purchases were correctly identified.

### F1 Score

Provides a balance between precision and recall.

### Confusion Matrix

Shows:

```text
True Positive
True Negative
False Positive
False Negative
```

---

## 📈 Graphical Analysis

The project generates several graphs.

### 1. Model Accuracy Comparison

Compares the accuracy of:

* Logistic Regression
* KNN
* SVM
* Decision Tree
* Random Forest

### 2. Age vs Estimated Salary

Shows the relationship between customer age and estimated salary.

### 3. Purchase Rate by Age Group

Analyzes purchase behavior across different age groups.

### 4. Purchase Rate by Salary Group

Analyzes purchase behavior across different salary groups.

### 5. Confusion Matrices

Confusion matrices are generated for the classification models.

---

## 🧪 Customer Prediction Scenarios

The project tests several customer profiles.

### Question 1

The following customers are tested:

| Age |                 Salary |
| --: | ---------------------: |
|  30 |                 87,000 |
|  40 | Average dataset salary |
|  40 |                100,000 |
|  50 | Average dataset salary |

For cases where salary is described as **"No Salary"**, the program uses the average salary of the dataset as a numerical placeholder.

---

### Question 2

The following scenarios are also tested:

| Age |                 Salary |
| --: | ---------------------: |
|  18 | Average dataset salary |
|  22 |                600,000 |
|  35 |              2,500,000 |
|  60 |            100,000,000 |

**Note:** Some of these salary values are far outside the range of the original dataset. Therefore, their results should be interpreted as **model extrapolations**, not strongly validated real-world predictions.

---

## 🔬 Hypothesis Testing

The project investigates the following assumptions.

### Hypothesis 1

**Younger customers with higher salaries may have a higher probability of purchasing.**

The model tests younger customers with relatively high salaries.

---

### Hypothesis 2

**Older customers with higher salaries may have different purchase behavior.**

The model compares older and younger customers with similar salary levels.

---

### Hypothesis 3

**Salary may have a strong influence on purchase prediction.**

Customers with the same age but different salary levels are compared.

The predictions from all five algorithms are examined.

---

## 💻 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook / Google Colab
* VS Code
* Git
* GitHub

---

## 📦 Python Libraries

Install the required libraries using:

```bash
pip install pandas numpy matplotlib scikit-learn
```

---

## ▶️ How to Run the Project

### Step 1: Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### Step 2: Open the Project

```bash
cd AI-Insurance-Purchase-Prediction
```

### Step 3: Install Dependencies

```bash
pip install pandas numpy matplotlib scikit-learn
```

### Step 4: Make Sure the Dataset Exists

The project folder should contain:

```text
AI-Insurance-Purchase-Prediction/
│
├── insurance_prediction.py
├── Social_Network_Ads.csv
└── README.md
```

### Step 5: Run the Program

```bash
python insurance_prediction.py
```

If you are using Windows and `python` does not work:

```bash
py insurance_prediction.py
```

---

## 📁 Project Structure

```text
AI-Insurance-Purchase-Prediction/
│
├── insurance_prediction.py
├── Social_Network_Ads.csv
├── README.md
└── graphs/
```

### File Description

| File                      | Purpose                             |
| ------------------------- | ----------------------------------- |
| `insurance_prediction.py` | Complete Machine Learning program   |
| `Social_Network_Ads.csv`  | Dataset                             |
| `README.md`               | Project documentation               |
| `graphs/`                 | Generated graphs and visualizations |

---

## 🧠 Key Learning Outcomes

Through this project, the following concepts are learned:

* Data preprocessing
* Feature selection
* Train-test splitting
* Feature scaling
* Classification
* Logistic Regression
* KNN
* SVM
* Decision Trees
* Random Forest
* Model evaluation
* Confusion matrices
* Data visualization
* Customer prediction
* Hypothesis testing
* Model comparison
* Git and GitHub project management

---

## 🌍 Real-Life Applications

Machine Learning classification models can be used in areas such as:

### 1. Insurance

Companies can analyze customer characteristics to estimate the likelihood of purchasing insurance products.

### 2. Banking

Banks can use customer information to predict interest in loans, credit cards, or other financial products.

### 3. Marketing

Companies can identify customer groups that may be more interested in specific products or services.

---

## 🚀 Future Improvements

The project can be improved by:

* Adding more customer features.
* Using larger and more diverse datasets.
* Performing hyperparameter tuning.
* Using cross-validation.
* Adding feature importance analysis.
* Deploying the model as a web application.
* Creating an interactive Streamlit dashboard.
* Adding real-time customer prediction.
* Using explainable AI techniques.
* Monitoring model performance on new data.

---

## ⚠️ Limitations

This project uses only two main input features:

```text
Age
Estimated Salary
```

Therefore, real-world insurance purchasing decisions may depend on many additional factors.

Predictions for salary values far outside the training-data range should be treated cautiously because they represent extrapolation.

The model should be considered an educational Machine Learning project rather than a real insurance decision-making system.

---

## 📌 Conclusion

This project demonstrates how Machine Learning classification algorithms can be applied to predict customer purchase behavior.

Five algorithms are implemented:

```text
Logistic Regression
KNN
Support Vector Machine
Decision Tree
Random Forest
```

Their performance is compared using multiple evaluation metrics. The project also uses graphical analysis and customer scenarios to study the relationship between age, estimated salary, and purchase behavior.

The project provides practical experience in **Machine Learning, data preprocessing, visualization, model evaluation, and GitHub-based project development**.

---

## 👩‍💻 Author

**Pragna S**

## ⭐ Project

If you find this project useful, consider giving the repository a ⭐ on GitHub.
