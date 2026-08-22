# 📊 Student Exam Performance Prediction

A machine learning project that predicts a student's **Mathematics score** based on demographic, educational, and previous exam performance features.

The project covers the complete machine learning workflow, from data preprocessing and exploratory data analysis to model training, evaluation, and deployment using Flask.

---

## 📌 Project Overview

The goal of this project is to build a machine learning model capable of predicting a student's mathematics score using information such as:

- Gender
- Race/Ethnicity
- Parental Level of Education
- Lunch Type
- Test Preparation Course
- Reading Score
- Writing Score

The trained model is integrated with a **Flask web application**, allowing users to enter student information and receive a predicted mathematics score.

---

## 🎯 Objective

The primary objective is to understand and implement a complete machine learning workflow:

```text
Raw Dataset
     ↓
Data Ingestion
     ↓
Data Cleaning & Preprocessing
     ↓
Exploratory Data Analysis
     ↓
Feature Transformation
     ↓
Model Training
     ↓
Model Evaluation
     ↓
Flask Deployment
     ↓
Mathematics Score Prediction
```

---

## 📂 Project Structure

```text
ML-project/
│
├── artifacts/
│   ├── data.csv
│   ├── train.csv
│   └── test.csv
│
├── notebook/
│   └── data/
│       └── stud.csv
│
├── src/
│   ├── components/
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   │
│   ├── exception.py
│   ├── logger.py
│   └── utils.py
│
├── templates/
│   └── home.html
│
├── static/
│   └── ...
│
├── application.py
├── requirements.txt
├── setup.py
├── README.md
└── .gitignore
```

---

## 📊 Dataset

The project uses a student performance dataset containing information about students' demographic characteristics, educational background, test preparation, and exam scores.

### Features

| Feature | Description |
|---|---|
| `gender` | Gender of the student |
| `race_ethnicity` | Student's race/ethnicity group |
| `parental_level_of_education` | Parent's highest level of education |
| `lunch` | Type of lunch received by the student |
| `test_preparation_course` | Whether the student completed a test preparation course |
| `reading_score` | Student's reading score |
| `writing_score` | Student's writing score |
| `math_score` | Student's mathematics score (target variable) |

### Target Variable

```text
math_score
```

The model attempts to predict the student's mathematics score.

---

## 🔍 Exploratory Data Analysis

Exploratory Data Analysis was performed to understand the relationships and patterns present in the dataset.

The analysis includes:

- Distribution of numerical features
- Categorical feature analysis
- Relationship between exam scores
- Correlation analysis
- Identification of potential outliers
- Understanding the target variable distribution

The purpose of EDA is not simply to generate visualizations, but to understand the dataset and identify patterns that may be useful during model development.

---

## 🧹 Data Preprocessing

The dataset contains both numerical and categorical features.

The preprocessing stage handles:

- Categorical feature encoding
- Numerical feature processing
- Feature transformation
- Train-test separation

The preprocessing pipeline ensures that the data is converted into a format suitable for machine learning models.

---

## 🤖 Machine Learning

The project evaluates machine learning models for predicting mathematics scores.

The general workflow is:

```text
Training Data
      ↓
Feature Transformation
      ↓
Model Training
      ↓
Predictions
      ↓
Evaluation
```

The trained model is then saved and used by the prediction pipeline.

---

## 🌐 Flask Application

The trained machine learning model is integrated into a Flask web application.

Users can enter:

- Gender
- Race/Ethnicity
- Parental education
- Lunch type
- Test preparation status
- Reading score
- Writing score

The application processes these inputs and returns a predicted mathematics score.

### Example

```text
Input
─────
Reading Score: 85
Writing Score: 88
Test Preparation: Completed
Lunch: Standard
...

        ↓

Machine Learning Model

        ↓

Predicted Mathematics Score
```

---

## 🚀 Running the Project Locally

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd ML-project
```

### 2. Activate the virtual environment

If using the existing Python virtual environment:

```powershell
.env\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Flask application

```bash
python application.py
```

The application should then be available at:

```text
http://127.0.0.1:5000/
```

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Matplotlib**
- **Seaborn**
- **Flask**
- **HTML/CSS**
- **Git/GitHub**

---

## 🧠 Key Concepts Practiced

This project helped explore several important machine learning concepts:

- Data ingestion
- Data cleaning
- Exploratory Data Analysis
- Feature transformation
- Categorical encoding
- Train-test splitting
- Regression
- Model evaluation
- Pipeline-based preprocessing
- Model persistence
- Flask model deployment
- Logging
- Custom exception handling
- Modular ML project structure

---

## 📈 Project Learning Outcomes

Through this project, I worked on understanding how a machine learning model moves beyond a notebook and becomes part of an application.

The project follows a modular structure:

```text
Data Ingestion
      ↓
Data Transformation
      ↓
Model Training
      ↓
Prediction Pipeline
      ↓
Flask Application
```

This structure separates different responsibilities of the machine learning workflow and makes the project easier to maintain and extend.

---

## 🔮 Future Improvements

Possible improvements include:

- Hyperparameter optimization
- Additional model evaluation
- Better model interpretability
- Improved frontend design
- Input validation
- Model performance monitoring
- Deployment to a cloud platform

---

## 👨‍💻 Author

**Moniish Mohan Srinivasan**

B.Tech Computer Science Engineering

---

## 📄 License

This project is intended for educational and learning purposes.
