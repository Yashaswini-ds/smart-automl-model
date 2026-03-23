# smart-automl-model
Smart AutoML system that trains multiple ML models, selects the best using hyperparameter tuning, and enables predictions using a saved pre-trained model without retraining.
# 🚀 Smart AutoML Model (Pre-trained ML System)

## 📌 Overview
This project implements a smart AutoML pipeline that automatically selects the best machine learning model from multiple algorithms using hyperparameter tuning.

The system trains once, saves the best model, and allows future predictions without retraining.

---

## ⚙️ Features
- Multiple ML models (Logistic Regression, Random Forest, SVM, KNN, Decision Tree)
- Hyperparameter tuning using GridSearchCV
- Feature selection using SelectKBest
- Model comparison visualization
- Pre-trained model saving and loading
- Reusable prediction system

---

## 🧠 Workflow
1. Load dataset
2. Train multiple models
3. Select best model automatically
4. Save trained model
5. Load model later for predictions

---

## 📊 Model Performance
The system compares multiple models and selects the best based on accuracy.

---

## 💾 Pre-trained Model
The trained model is saved as:

best_model.pkl

You can directly load and use it without retraining.

---

## 🔮 Example Usage

```python
import joblib

model = joblib.load("best_model.pkl")
prediction = model.predict(input_data)
