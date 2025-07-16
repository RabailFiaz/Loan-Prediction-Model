# 🏦 Loan Prediction Web Application

### Developed by:
- **Rabail Fiaz** – Reg. No: L1F22BSCS1096  
- **Areeba Binte Mahtab** – Reg. No: L1F22BSCS1109  
- **Jahanzaib Ahmed** – Reg. No: L1F22BSCS1115  

---

## 📌 Project Description

This is a machine learning-based web application that predicts whether a loan should be approved for a customer based on their financial and personal information.

The model uses the **Gaussian Naive Bayes** algorithm, trained on a public dataset. The prediction system is deployed through an **interactive Streamlit web interface** to simulate a banking decision-support system for loan approvals.

---

## 💡 Key Features

### ✅ Streamlit Web Interface
- Clean and interactive layout for user input
- Real-time prediction with a click of a button

### 🧾 Inputs Collected
- Gender  
- Marital Status  
- Education  
- Self Employment  
- Applicant Income  
- Co-applicant Income  
- Loan Amount  
- Loan Amount Term  
- Credit History  
- Property Area  

### 🧠 Prediction
- Predicts loan approval status using a trained **Gaussian Naive Bayes** model
- Outputs result instantly as **"Approved"** or **"Not Approved"**

---

## 📊 Dataset Information

- **Source:** Kaggle (Loan Prediction Dataset) or similar open datasets
- **Target Variable:** `Loan_Status` (Yes = Approved, No = Not Approved)
- **Used Features:**
  - Gender, Married, Education, Self_Employed  
  - ApplicantIncome, CoapplicantIncome, LoanAmount  
  - Loan_Amount_Term, Credit_History, Property_Area

### 🔧 Data Preprocessing
- Label Encoding for categorical values
- Missing value handling (imputation)
- Feature scaling (if needed)
- Train-test split (e.g., 80-20 ratio)

---

## 🧠 Machine Learning Model

### 🔍 Algorithm Used
**Gaussian Naive Bayes**

### ✅ Why Gaussian Naive Bayes?
- Efficient and fast training
- Suitable for small-to-medium tabular datasets
- Assumes feature independence (valid for this dataset)

### 🔁 ML Pipeline
1. Data cleaning and preprocessing
2. Label encoding for categorical features
3. Model training using `GaussianNB()`
4. Evaluation using:
   - Accuracy
   - Confusion matrix
5. Saving the model with `joblib`
6. Streamlit integration for live use

---

## 📈 Project Outcomes

- Achieved prediction **accuracy around 80%**
- Fast real-time results for loan decisions
- Minimal latency and light memory usage
- User-friendly interface for non-technical users

---

## 🗂 Project Structure

Loan-Prediction-Model/
│
├── dataset/
│ └── loan_data.csv
│
├── model/
│ └── loan_model.pkl
│
├── app.py # Streamlit frontend
├── model_training.py # Model training script
├── requirements.txt # Python dependencies
└── README.md # Project documentation


---

## ⚙️ How to Run Locally

### Step 1: Clone the repository


```bash
git clone https://github.com/RabailFiaz/Loan-Prediction-Model.git
cd loan-prediction-app
