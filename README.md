# 🚢 Titanic Survival Prediction

A machine learning project that predicts whether a passenger survived the Titanic disaster based on personal and travel-related attributes.

---

## 📌 Problem

The sinking of the RMS Titanic is one of the most well-known shipwrecks in history. Out of 2,224 passengers and crew, more than 1,500 lost their lives. Interestingly, survival was not random — factors like age, gender, passenger class, and fare played a major role.

**Goal:**
Build a predictive model that answers:

> **“Given a passenger’s details, can we predict whether they survived or not?”**

This is a **binary classification problem** where:

* **1 = Survived**
* **0 = Did Not Survive**

---

## 🧠 Approach

The project follows a complete end-to-end machine learning workflow:

### 1. Data Understanding

Dataset includes passenger-level features such as:

* Passenger class (Pclass)
* Gender (Sex)
* Age
* Number of siblings/spouses aboard (SibSp)
* Number of parents/children aboard (Parch)
* Fare
* Embarked port

Exploratory Data Analysis (EDA) was performed to:

* Understand survival distribution
* Identify key survival patterns (e.g., women and children had higher survival rates)
* Detect missing values and outliers

---

### 2. Data Preprocessing

* Handled missing values (Age, Embarked, etc.)
* Encoded categorical features (Sex, Embarked)
* Feature scaling (where required)
* Feature engineering (e.g., Family Size = SibSp + Parch + 1)

---

### 3. Model Building

Multiple classification algorithms were tested, such as:

* Logistic Regression
* Decision Tree
* Random Forest
* (Optional) Gradient Boosting / XGBoost

The dataset was split into training and testing sets to evaluate model performance.

---

### 4. Model Evaluation

Performance was measured using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

Hyperparameter tuning was performed to improve generalization.

---

## 📊 Results

* The model successfully learned survival patterns from passenger attributes.
* Features like **Sex, Pclass, Age, and Fare** had strong influence on predictions.
* The final model achieved strong classification performance on the test dataset, showing good balance between precision and recall.
* The system can now predict survival probability for a new passenger record.

---

## 🛠 Tech Stack

| Category         | Tools / Libraries          |
| ---------------- | -------------------------- |
| Language         | Python                     |
| Data Handling    | Pandas, NumPy              |
| Visualization    | Matplotlib, Seaborn        |
| ML Models        | Scikit-learn               |
| Model Evaluation | Scikit-learn Metrics       |
| Environment      | Jupyter Notebook / VS Code |

