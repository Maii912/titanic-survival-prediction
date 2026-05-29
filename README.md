# 🚢 Titanic Survival Prediction using Machine Learning

This repository contains a Python-based machine learning project that predicts whether a passenger survived the Titanic shipwreck based on features like age, sex, passenger class, and more. 

The project uses the classic Kaggle Titanic dataset and implements a workflow in a Jupyter Notebook.

---

## 📊 Project Workflow & Code Structure

The project follows a standard data science pipeline:

1. **Data Exploration & Analysis:** - Loaded and inspected the dataset using `pandas`.
   - Identified missing values in columns like `Age`, `Cabin`, and `Embarked`.
2. **Data Cleaning & Feature Selection:**
   - Dropped irrelevant columns that do not contribute to prediction (`Name`, `Ticket`, `Cabin`, `PassengerId`).
   - Imputed missing values: Filled missing `Age` values with the mean, and missing `Embarked` values with the mode.
3. **Categorical Encoding:**
   - Used `LabelEncoder` from Scikit-Learn to convert categorical text features (`Sex` and `Embarked`) into numerical values.
4. **Model Training:**
   - Split the data into training and testing sets (80% train, 20% test).
   - Trained a **Random Forest Classifier** model on the preprocessed training data.
5. **Evaluation:**
   - Evaluated the model using the test set.

---

## 📈 Results

- **Model Used:** Random Forest Classifier
- **Accuracy Score:** **80.44%** (`0.8044692737430168`)

---

## 🛠️ Tech Stack & Libraries Used

The following Python libraries are required to run this project:

- **Data Manipulation:** `pandas`, `numpy`
- **Machine Learning:** `scikit-learn`
  - `LabelEncoder` (Preprocessing)
  - `train_test_split` (Model Selection)
  - `RandomForestClassifier` (Ensemble Model)
  - `accuracy_score` (Metrics)

---

## 📦 How to Run the Project

1. Clone this repository to your computer.
2. Ensure you have Jupyter Notebook or VS Code installed.
3. Install the required packages via terminal if you haven't already:
   ```bash
   pip install pandas numpy scikit-learn