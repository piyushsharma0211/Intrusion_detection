# Intrusion Detection System using CICIDS2017 Dataset

## 📌 Overview
This project implements an **Intrusion Detection System (IDS)** using the **CICIDS2017** dataset to detect and classify malicious network activities.  
It applies **data preprocessing**, **dimensionality reduction**, and **machine learning classification models** to identify both binary (Normal vs. Attack) and multi-class attack categories.

The system is built with **Python**, leverages **scikit-learn** for ML models, and applies techniques like **SMOTE** for class imbalance handling and **Incremental PCA** for feature reduction.

---

## 📂 Dataset
The dataset used is **CICIDS2017**, which contains realistic network traffic data for various attack types such as DoS, DDoS, Brute Force, Botnet, Port Scans, and more.  
🔗 **Dataset Link:** [CICIDS2017 Google Drive](https://drive.google.com/drive/folders/1MmaRbhLKoBKLFmlC5HVRysUuhvGB7jiC?usp=sharing)

---

## 🛠 Features
- **Data Preprocessing**
  - Remove duplicates, missing values, infinite values
  - Handle zero-variance features
  - Outlier detection and removal
  - Downcasting for memory optimization
- **Feature Engineering**
  - Dimensionality reduction using **Incremental PCA**
  - Class imbalance handling with **SMOTE**
- **Model Training**
  - Binary Classification:
    - Logistic Regression
    - Support Vector Machine (SVM)
  - Multi-class Classification:
    - Random Forest
    - Decision Tree
    - K-Nearest Neighbors (KNN)
- **Evaluation**
  - Accuracy, Recall, F1-score
  - Confusion Matrix
  - Cross-validation

---

## 🏗 Project Structure
IDS-CICIDS2017/
│
├── data/ # Dataset files (not included in repo, download from link)
├── notebooks/ # Jupyter Notebooks for EDA, preprocessing, and model training
├── scripts/ # Python scripts for modularized code
├── models/ # Saved trained models (.pkl files)
├── results/ # Confusion matrices, plots, performance metrics
├── requirements.txt # Python dependencies
├── README.md # Project documentation
└── main.py # Main script to run the IDS pipeline

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/piyushsharma0211/Intrusion_detection.git
cd Intrusion_detection

📊 Results (Example)
Model	Accuracy	Recall	F1-score
Logistic Regression	97.3%	96.8%	97.0%
SVM	98.1%	97.5%	97.8%
Random Forest	99.2%	99.0%	99.1%

(Values are based on our trained models; your results may vary.)

📌 Future Improvements
Add deep learning models (LSTM, CNN) for better accuracy

Deploy the IDS as a real-time network monitoring tool

Integrate with cloud services for large-scale data handling

