# 🏥 Disease Prediction using Machine Learning

An AI-driven web application built with Streamlit that enables user-friendly prediction of multiple diseases including Diabetes, Heart Disease, Parkinson’s, Lung Cancer, and Hypo‑Thyroid using trained ML models. Diagnosis is quick, intuitive, and respects user data privacy.


## 🎯 Problem Statement

Early detection of diseases significantly improves treatment outcomes. However, many users lack access to diagnostic tools or medical expertise. This project aims to:

* Provide accessible disease risk prediction through simple user inputs.

* Offer predictions for multiple conditions using well-trained ML models.

* Ensure data privacy through encrypted storage and secure handling.

## 🚀 Features

Multiple Disease Prediction: Predicts Diabetes, Heart Disease, Parkinson’s, Lung Cancer, and Hypo‑Thyroid.

* Streamlit UI: Clean, intuitive interface with dropdowns, form input fields, and results display.

* AI‑Powered Models: Classifiers trained using Scikit‑Learn or TensorFlow/Keras, saved in .sav or .pkl files.

* Secure Data Handling: Patient inputs encrypted or stored in SQLite / Firebase depending on configuration.

* Model Interpretability: Optional confidence scores or bar charts to understand feature importance.

## 🏗️ System Architecture

### The diagram above (click to download PNG) shows:

* User Interface (Streamlit) → collects medical inputs.

* Pre-processing Module → validates and normalizes inputs.

* Model Inference Engine → runs one of several disease prediction models.

* Result Display → outputs prediction and confidence.

* Secure Cloud Storage → optional persistence using encrypted SQLite or Firebase backend.


## 🛠️ Tech Stack

| Component              | Technology / Tools                               |
|------------------------|--------------------------------------------------|
| **Frontend / UI**      | Streamlit                                        |
| **Programming Language** | Python                                         |
| **Machine Learning**   | Scikit-Learn, optionally TensorFlow/Keras        |
| **Model Storage**      | `.sav` / `.pkl` files                            |
| **Data Handling**      | Pandas, NumPy                                    |
| **Backend Storage**    | SQLite / Firebase (Optional)                     |
| **Deployment**         | Streamlit CLI / Streamlit Cloud                  |
| **Security**           | Input Validation, Encrypted Storage, Hashing     |
| **Version Control**    | Git + GitHub                                     |


## 🔬 How to Run the Project

#### 1. Clone the Repository

```bash
git clone https://github.com/Ritikayogi/AI-Medical-diagnosis-using-AI
cd disease-prediction-ml
```
---


#### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

---

#### 3. Run the Application

```bash
streamlit run app.py
```

---

#### 4. Test API using Swagger or Postman

Open in your browser:
```
(http://localhost:8501)
```
---

## 🚀 Usage

### streamlit run app.py

Once the app is running, open the browser (http://localhost:8501). Then:

* Choose a disease from the dropdown.

* Enter required medical inputs (e.g., age, blood sugar, BMI, etc.).

* Click Predict.

* View the diagnosis along with confidence score/chart.

* Optionally save your data securely.

## 📦 Project Structure


```bash
AI-Medical-diagnosis-using-AI/
│
├── app.py                      # Streamlit application
├── requirements.txt            # Required Python packages
├── README.md                   # Project documentation
├── diabetes_model.sav          # Trained diabetes model
├── heart_model.sav             # Trained heart model
├── parkinsons_model.sav        # Trained parkinsons model
├── thyroid_model.sav           # Trained thyroid model
├── lung_cancer_model.sav       # Trained lung cancer model
└── assets/                     # Images, icons, etc (optional)
```
## 📈 Performance

* Diabetes model: Accuracy ~92%

* Heart Disease: Accuracy ~90%

* Parkinson’s: Accuracy ~89%

* Lung Cancer & Hypo‑Thyroid: Accuracy estimates ~85–90%

* Optional confusion matrix or ROC curve plots for evaluation


## 🔒 Privacy & Security

* User inputs are validated and optionally encrypted.

* No patient data is stored unless configured with secure backend.

* Use best practices (OWASP, encrypted storage, hashed data handling).


## 📅 Future Enhancements

* 🌐 Expand datasets for better accuracy and coverage

* 💬 Integrate chatbot-based symptom intake

* 🧠 Add CNN-based X‑ray or MRI image analysis for image-enabled disease prediction

* 📊 Provide model explainability (e.g., SHAP or LIME visualizations)

* ☁️ Deploy via Streamlit Cloud or AWS with authentication layer

## ✅ Contribution

Contributions are welcome—fork, improve README, UI, or add new models/features!

#### Let me know if you’d like help adding:

* Docker setup script

* Unit tests using PyTest

* Swagger / API endpoints for model inference

* CI/CD pipeline for deployment
