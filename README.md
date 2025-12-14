# 🚿 SciShower ML  
### **Scientific Shower Temperature Recommendation System**  
**Developed by: Srivatsan MK**

SciShower ML is a machine learning–powered system that predicts the **ideal shower water temperature** for a user based on multiple scientific and environmental factors such as weather, mood, activity, personal preference, and thermal comfort science.

This project uses a **Random Forest Regression Model**, trained on a **20,000-row scientifically-informed dataset**, and provides a clean **HTML/CSS frontend** with a **Flask backend** to generate real-time temperature recommendations.

---

## 📌 **Features**

- ✔ Predict ideal shower temperature (in °C)  
- ✔ Uses scientifically modeled dataset  
- ✔ Machine learning model trained using Random Forest  
- ✔ HTML/CSS modern light-themed UI  
- ✔ Flask backend for real-time predictions  
- ✔ Clean, responsive, and user-friendly interface  
- ✔ Perfect dataset: 20,000+ rows and 17 features  
- ✔ Easy to deploy and customize  

---

## 📊 **Dataset Overview**

The dataset contains **20,000 scientifically informed records** with features such as:

- Month  
- Season  
- Time of day  
- Hour  
- Outside temperature & humidity  
- Rain status  
- Gender  
- Age group  
- Heat preference  
- Activity before shower  
- Mood  
- Health status  
- Last shower temperature  
- Average last 7 days temperature  
- **Target:** Recommended shower temperature (°C)

---

## 🧠 **Machine Learning**

Model used: **Random Forest Regressor**

### ML Pipeline:
1. Data preprocessing  
2. OneHotEncoding (categorical data)  
3. Standard Scaling (numerical data)  
4. Training Random Forest model  
5. Model evaluation (MAE, RMSE)  
6. Saving model as `.pkl` file  

---

## 🧪 **Technologies Used**

- **Python**
- **Flask**
- **Pandas / NumPy**
- **Scikit-Learn**
- **HTML5 / CSS3**
- **Joblib**

---

## 📂 **Project Structure**
```
SciShower-Project/
│
├── app.py
├── requirements.txt
├── models/
│ └── shower_temp_model.pkl
├── templates/
│ ├── index.html
│ └── result.html
├── static/
│ ├── style.css
│ └── result.css
├── data/
│ └── shower_temperature_20k_dataset.csv
└── src/
└── train_model.py
```

---

## ⚙️ **Installation Guide**

### 1. Clone the repository
```bash
git clone <your-repo-link>
cd SciShower-Project
```
### 2. Create Virtual Environment
```
python -m venv venv
```
### 3.Activate Environment
Windows
```
venv\Scripts\activate
```
### 4. Install Dependencies
```
pip install -r requirements.txt
```

---

### 🤖 Train the Model (Optional)
If you want to retrain:
```
python src/train_model.py
```
This generates:
```
models/shower_temp_model.pkl
```

---

### 🚀 Run the Flask App
```
python app.py
```
Then open http://127.0.0.1:5000 in your browser.

---
### 🎯 How It Works

- User fills the form
- Flask receives data (POST)
- Model predicts ideal shower temperature
- Result shown on a separate output page
