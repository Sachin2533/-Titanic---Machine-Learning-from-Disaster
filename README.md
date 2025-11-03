# 🛳️ Titanic Survival Prediction

## 📘 Project Overview  
This project predicts the survival of passengers aboard the **RMS Titanic** using machine learning.  
It’s based on the classic **Kaggle Titanic Dataset**, which contains details such as age, sex, passenger class, and family information.  
The goal is to train a model that accurately determines whether a passenger survived or not.

---

## ⚙️ Data Preprocessing  
- **Handled Missing Values**
  - Replaced missing `Age` values with the mean.
  - Filled missing `Embarked` values with the most frequent value (mode).
- **Feature Encoding**
  - Converted categorical columns (`Sex`, `Embarked`) into numerical format using `pd.get_dummies()`.
- **Feature Selection**
  - Removed non-essential columns: `Name`, `Ticket`, `Cabin`, `SibSp`, and `Parch`.
- **Data Splitting**
  - Split the dataset into **80% training** and **20% validation** sets for evaluation.

---

## 🤖 Model Used  
A **Random Forest Classifier** from Scikit-learn was trained on the processed data.  
The model achieved an approximate **validation accuracy of 83%**.

After validation, the same trained model was used to generate predictions on the **test dataset** for submission.

---

## 📈 Output  
The predictions were saved in a file named **`submission.csv`** containing the following columns:
| Column | Description |
|---------|--------------|
| PassengerId | Unique ID of the passenger |
| Survived | 0 = Did not survive, 1 = Survived |

This file can be directly uploaded to the **Kaggle Titanic competition** for scoring.

---

## 🧩 Technologies Used  
- 🐍 **Python 3**
- 📊 **Pandas** – Data manipulation  
- 🔢 **NumPy** – Numerical operations  
- 📉 **Matplotlib** & **Seaborn** – Data visualization  
- 🧠 **Scikit-learn** – Machine learning model (Random Forest Classifier)

---




