# 🩺 AI-Powered Healthcare Analysis  
### Member 1 – Data Scientist: Hafsa Hajir  

This project demonstrates how **machine learning using Scikit-learn** can predict diabetes risk based on key patient health indicators.  
It is part of a larger group assignment under the theme **“Mastering the AI Toolkit”**, focusing on applying different AI tools to solve real-world healthcare problems.

---

## 📋 Project Overview  

The objective of this work is to build a **baseline predictive model** that determines the likelihood of diabetes in patients using structured healthcare data.  
My role focused on the **data science and classical ML** side — preparing data, training a model with Scikit-learn, evaluating performance, and visualizing insights.

**Theme:** *Mastering the AI Toolkit – Healthcare Applications*  
**Dataset:** *Pima Indians Diabetes Dataset (Kaggle)*  
**Framework:** *Scikit-learn*

---

## 👩🏽‍💻 My Role  

As the **Data Scientist**, my responsibilities included:  
- 🧹 Cleaning and preparing the dataset  
- 📊 Performing exploratory data analysis (EDA)  
- ⚙️ Building and training a baseline model using `RandomForestClassifier`  
- 📈 Evaluating model performance  
- 🔍 Visualizing feature importance and drawing insights  

---

## 🧰 Tools and Libraries Used  

- **Python**  
- **Pandas** – data handling  
- **NumPy** – numerical operations  
- **Scikit-learn** – machine learning model building  
- **Matplotlib / Seaborn** – visualization  

---

## 📊 Dataset Description  

**Name:** Pima Indians Diabetes Dataset  
**Source:** [Kaggle – Diabetes Dataset](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)  

**Features:**
- Pregnancies  
- Glucose  
- BloodPressure  
- SkinThickness  
- Insulin  
- BMI  
- DiabetesPedigreeFunction  
- Age  
- Outcome *(Target: 1 = Diabetic, 0 = Non-Diabetic)*  

---

## 💻 Model Implementation  

```python
# Import libraries
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score, classification_report
import matplotlib.pyplot as plt

# Load dataset
url = "https://raw.githubusercontent.com/jbrownlee/Datasets/master/pima-indians-diabetes.data.csv"
columns = ['Pregnancies', 'Glucose', 'BloodPressure', 'SkinThickness', 
           'Insulin', 'BMI', 'DiabetesPedigreeFunction', 'Age', 'Outcome']
df = pd.read_csv(url, names=columns)

# Split data
X = df.drop('Outcome', axis=1)
y = df['Outcome']

X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)

# Scale features
scaler = StandardScaler()
X_train = scaler.fit_transform(X_train)
X_test = scaler.transform(X_test)

# Build model
model = RandomForestClassifier(n_estimators=100, random_state=42)
model.fit(X_train, y_train)

# Evaluate model
y_pred = model.predict(X_test)

print("Accuracy:", accuracy_score(y_test, y_pred))
print("\nClassification Report:\n", classification_report(y_test, y_pred))

# Feature Importance
importances = model.feature_importances_
plt.barh(columns[:-1], importances)
plt.title("Feature Importance in Diabetes Prediction")
plt.show()
