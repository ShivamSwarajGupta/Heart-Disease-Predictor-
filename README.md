# Heart Disease Prediction - ML Basics & Data Preprocessing

This repository contains a Google Colab notebook that introduces **Machine Learning basics and data preprocessing** using a **Heart Disease Dataset** from Kaggle.  
It is designed as **Day 1** of an ML learning journey, focusing on preparing data for machine learning tasks.

---

## 📌 Project Overview
- Learn how to use **Google Colab** for ML projects.  
- Connect Kaggle API to Colab for dataset downloads.  
- Perform **data preprocessing** (handling missing values, feature selection, encoding, etc.).  
- Explore **basic ML algorithms** for classification.  

The dataset used is **Heart Disease UCI Dataset**, which contains patient medical records to predict the likelihood of heart disease.

---

## 📂 Dataset
- Source: [Heart Disease Dataset (Kaggle)](https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data)  
- File: `heart_disease_uci.csv`  
- Features include age, sex, chest pain type, blood pressure, cholesterol, etc.  
- Target: Presence of **heart disease** (binary classification).  

---

## ⚙️ Setup Instructions

### 1. Upload Kaggle API key
- Download your `kaggle.json` from [Kaggle API](https://www.kaggle.com/docs/api).  
- Upload it inside the Colab session:

```python
from google.colab import files
files.upload()  # Upload kaggle.json
```

### 2. Configure Kaggle
```bash
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
!pip install kaggle
```

### 3. Download Dataset
```bash
!kaggle datasets download -d redwankarimsony/heart-disease-data -p /content/heart-disease --unzip
```

---

## 🚀 Running the Notebook
1. Open the notebook in [Google Colab](https://colab.research.google.com/).  
2. Run the setup cells to configure Kaggle API and download the dataset.  
3. Explore data preprocessing and ML steps included in the notebook.  

---

## 📊 Topics Covered
- Dataset loading & inspection with **pandas**.  
- Data cleaning and preprocessing.  
- Feature engineering basics.  
- Exploratory Data Analysis (EDA).  
- Basic ML model building.  

---

## ✅ Requirements
The notebook automatically installs most dependencies in Colab.  
Key packages:  
- `pandas`  
- `numpy`  
- `scikit-learn`  
- `matplotlib` / `seaborn`  
- `kaggle` (for dataset download)  

---

## 📌 Future Improvements
- Add more advanced ML models (Logistic Regression, Random Forest, etc.).  
- Improve visualization for insights.  
- Deploy a simple prediction model.  

---
