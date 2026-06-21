# Introduction to Machine Learning

## What is Machine Learning?

Machine Learning (ML) is a branch of Artificial Intelligence (AI) that enables computers to learn patterns from data and make predictions or decisions without being explicitly programmed for every scenario.

### Traditional Programming

Rules + Data → Output

Example:

```python
if temperature > 30:
    print("It's hot")
```

The rules are manually written by the programmer.

### Machine Learning

Data + Output → Model (Learns Rules)

Example:
Suppose we have data:

| Hours Studied | Passed |
| ------------- | ------ |
| 1             | No     |
| 2             | No     |
| 5             | Yes    |
| 7             | Yes    |

The machine learns the relationship between study hours and exam results and can predict outcomes for new students.

---

# Why Do We Need Machine Learning?

Traditional programming struggles when:

* The rules are too complex.
* Data changes frequently.
* The dataset is very large.
* Patterns are hidden and difficult for humans to identify.

Machine Learning can automatically discover these patterns.

Examples:

* Netflix movie recommendations
* Email spam detection
* Customer churn prediction
* Credit card fraud detection
* Self-driving cars
* Chatbots like ChatGPT

---

# What is Data?

Data is information that the model uses to learn patterns.

Example:

| Age | Salary | Purchased |
| --- | ------ | --------- |
| 25  | 30000  | No        |
| 35  | 60000  | Yes       |
| 42  | 80000  | Yes       |

Age and Salary are called Features (Inputs).

Purchased is called the Target Variable (Output).

---

# Important Terminologies

## 1. Features (X)

Features are input variables used to make predictions.

Examples:

* Age
* Salary
* Experience
* Monthly Charges
* Tenure

Features are usually represented by X.

---

## 2. Target Variable (y)

The target variable is what we want to predict.

Examples:

* Purchased (Yes/No)
* House Price
* Customer Churn
* Spam or Not Spam

The target variable is usually represented by y.

---

## 3. Dataset

A dataset is a collection of observations.

Example:

| Age | Salary | Purchased |
| --- | ------ | --------- |
| 25  | 30000  | No        |
| 35  | 60000  | Yes       |
| 42  | 80000  | Yes       |

Rows are called Observations or Samples.

Columns are called Features.

---

## 4. Model

A model is a mathematical representation that learns patterns from data.

Example:
A model learns:

Higher salary + more experience → Higher probability of purchase.

After training, the model can make predictions on new data.

---

# Types of Machine Learning

## 1. Supervised Learning

The model learns from labeled data.

Input → Correct Output is available.

Examples:

* House price prediction
* Customer churn prediction
* Email spam detection

Algorithms:

* Linear Regression
* Logistic Regression
* Decision Tree
* Random Forest
* XGBoost

Example:

Features:

* Monthly Charges
* Tenure

Target:

* Churn (Yes/No)

The model learns the relationship and predicts whether a customer will churn.

---

## 2. Unsupervised Learning

The model learns from unlabeled data.

No correct output is provided.

Goal:
Find hidden patterns in data.

Examples:

* Customer segmentation
* Market basket analysis
* Anomaly detection

Algorithms:

* K-Means Clustering
* Hierarchical Clustering
* DBSCAN
* PCA

---

## 3. Reinforcement Learning

An agent learns by interacting with an environment.

The agent receives rewards and penalties.

Goal:
Maximize cumulative reward.

Examples:

* Self-driving cars
* Chess engines
* Robotics
* Game AI

Components:
Agent → Takes Action → Receives Reward → Learns Better Actions

---

# Machine Learning Workflow

Step 1: Collect Data
↓
Step 2: Clean and Preprocess Data
↓
Step 3: Perform Exploratory Data Analysis (EDA)
↓
Step 4: Select Features
↓
Step 5: Train Model
↓
Step 6: Evaluate Model
↓
Step 7: Tune Hyperparameters
↓
Step 8: Deploy Model
↓
Step 9: Monitor and Improve

---

# Real Example: Customer Churn Prediction

Problem:
Predict whether a customer will leave the company.

Features:

* Tenure
* Monthly Charges
* Contract Type
* Internet Service

Target:
Churn (Yes/No)

Workflow:
Collect Data
→ Clean Data
→ Encode Categories
→ Train XGBoost
→ Evaluate using Precision, Recall, F1-score, ROC-AUC
→ Deploy Model

---

# Key Takeaways

1. Machine Learning enables systems to learn patterns from data.
2. Features are inputs and targets are outputs.
3. A model learns relationships between features and targets.
4. Machine Learning can be Supervised, Unsupervised, or Reinforcement Learning.
5. Every ML project follows a pipeline: Data → Preprocessing → Training → Evaluation → Deployment.
