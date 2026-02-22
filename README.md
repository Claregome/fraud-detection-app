Fraud Detection Prediction App

An end-to-end Machine Learning Fraud Detection System built with Python and deployed using Streamlit.
The model was trained on a financial transaction dataset containing over 6 million records and achieved 94% accuracy.

🚀 Project Overview

This project focuses on detecting fraudulent financial transactions using machine learning. It demonstrates the complete data science workflow:

Exploratory Data Analysis (EDA)

Data preprocessing & cleaning

Feature engineering

Handling class imbalance

Model training & evaluation

Model deployment with Streamlit

The final output is an interactive web application that allows users to input transaction details and receive real-time fraud predictions.

📊 Dataset Summary

6+ million transaction records

Transaction types include:

Cash In

Cash Out

Transfer

Payment

Fraud cases represent only 0.13% of total transactions, creating a significant class imbalance challenge.

🔎 Exploratory Data Analysis

Key insights from the analysis:

Cash-out and transfer transactions had the highest fraud rates.

Severe class imbalance required special modeling techniques.

Higher transaction amounts showed stronger correlation with fraud.

Outliers detected (maximum transaction value ≈ 92 million).

Correlation analysis revealed relationships between transaction amount and account balances.

Data visualization was performed using Matplotlib and Seaborn to better understand fraud patterns.

🤖 Machine Learning Model

Algorithm Used: Logistic Regression

Preprocessing Steps:

Train-Test Split

StandardScaler for feature scaling

Pipeline integration for clean workflow

Class imbalance handled using class_weight="balanced"

Model Performance:

✅ 94% Accuracy

Effective fraud detection despite severe imbalance

The trained model was exported using Joblib and integrated into the Streamlit app for predictions.

🌐 Streamlit Web Application

The project includes an interactive Streamlit web application.

Features:

User inputs for:

Transaction type

Transaction amount

Old balance (origin)

New balance (origin)

Old balance (destination)

New balance (destination)

Real-time fraud prediction

Simple and intuitive user interface

🛠️ Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Joblib

Streamlit

Jupyter Notebook

📂 Project Structure
Fraud-Detection-App/
│
├── data/
├── notebook/
│   └── fraud_analysis.ipynb
├── model/
│   └── fraud_pipeline.pkl
├── app.py
├── requirements.txt
└── README.md
⚙️ Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/your-username/fraud-detection-app.git
cd fraud-detection-app
2️⃣ Create virtual environment (recommended)
python -m venv venv
venv\Scripts\activate   # On Windows
3️⃣ Install dependencies
pip install -r requirements.txt
4️⃣ Run the Streamlit app
streamlit run app.py
📌 Key Skills Demonstrated

Large-scale data analysis (6M+ records)

Handling imbalanced datasets

Feature engineering

Machine learning pipeline creation

Model evaluation & validation

Model serialization (Joblib)

Web app deployment

End-to-end ML workflow

📈 Future Improvements

Experiment with advanced models (Random Forest, XGBoost)

Improve precision and recall for fraud class

Deploy to cloud platforms

Add monitoring and logging for real-world use

👩‍💻 Author

Clare Gome
Aspiring Data Scientist | Machine Learning Enthusiast

If you'd like, I can also create:

A version with GitHub badges

A more technical recruiter-focused version

Or a shorter, more concise README
