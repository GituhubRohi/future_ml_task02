# future_ml_task02
Machine Learning project for automatic support ticket classification and priority prediction

## 📌 Project Overview

Customer support teams receive hundreds of tickets every day. Manually sorting these tickets into categories and assigning priority takes time and may delay urgent issues.

This project builds a **Machine Learning system** that automatically:

* Classifies support tickets into categories
* Assigns a priority level (High / Medium / Low / Critical)

The goal is to help companies respond faster and improve customer satisfaction.

## 🎯 Objectives

The system reads customer support tickets and automatically:

1. **Classifies the ticket type**

   * Technical Issue
   * Billing Inquiry
   * Account Access
   * General Query

2. **Predicts ticket priority**

   * Critical
   * High
   * Medium
   * Low

## 🧠 Machine Learning Workflow

Support Ticket Text
↓
Text Cleaning (Lowercase, Stopword Removal)
↓
Feature Extraction using **TF-IDF**
↓
Machine Learning Model (Logistic Regression)
↓
Ticket Type Prediction
↓
Priority Prediction

## 🛠 Technologies Used

* Python
* Pandas
* NumPy
* NLTK (Natural Language Processing)
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

## 📊 Dataset

The dataset contains customer support tickets with:

* Ticket Text
* Ticket Type
* Ticket Priority

Example:

| Text                       | Ticket Type     | Ticket Priority |
| -------------------------- | --------------- | --------------- |
| Cannot login to account    | Account Access  | High            |
| Payment not processed      | Billing Inquiry | Medium          |
| System crashing during use | Technical Issue | Critical        |

Dataset Source: Kaggle Customer Support Ticket Dataset

##  Model Implementation

### Text Preprocessing

* Convert text to lowercase
* Remove punctuation
* Remove stopwords
* Tokenization using NLTK

### Feature Extraction

Text is converted to numerical features using **TF-IDF Vectorization**.

### Model Training

We use **Logistic Regression** to train two models:

1. Ticket Type Classification Model
2. Ticket Priority Prediction Model

## 📈 Model Evaluation

The model performance is evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

These metrics help understand how well the model predicts ticket categories and priorities.

## 🧪 Example Prediction

Input Ticket:
I cannot access my account and keep getting login errors.

Predicted Output:

Ticket Type → Account Access
Priority → High

## 💡 Business Impact

This system helps businesses:

* Automatically organize incoming support tickets
* Identify urgent issues faster
* Reduce manual ticket sorting
* Improve response time and customer satisfaction

## 📂 Project Structure

support-ticket-classification
│
├── dataset.csv
├── ticket_classification.ipynb
├── README.md

## 🚀 Future Improvements

* Deep learning models for better NLP performance
* Real-time ticket classification API
* Integration with customer support platforms
* Web dashboard for ticket monitoring

## 👩‍💻 Author
Rohini
Machine Learning Project developed as part of a hands-on learning task.

## ⭐ Acknowledgement

This project was completed as part of a Machine Learning task provided by **Future Interns**.

