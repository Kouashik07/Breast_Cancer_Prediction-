# 🩺 Breast Cancer Prediction (ML Project)

## 📌 Overview
This project predicts whether a breast tumor is **benign** or **malignant** using the **Breast Cancer Wisconsin (Diagnostic) Dataset**.  
The goal is to analyze tumor features such as **radius, texture, perimeter, area, smoothness, compactness, concavity, concave points, symmetry, and fractal dimension** to build a **Logistic Regression model** that can assist in early detection of breast cancer.

## 🔧 Tech Stack
- Python
- Pandas, NumPy
- Seaborn, Plotly, Matplotlib
- Scikit-Learn (Logistic Regression, preprocessing)

## 🚀 Project Workflow
1. **Data Exploration (EDA)**  
   - Checked feature distributions (mean, worst, SE)  
   - Analyzed relationships between features and diagnosis  
   - Correlation heatmaps to identify highly correlated features  

2. **Data Preprocessing**  
   - Dropped unnecessary columns (`id`, `Unnamed: 32`)  
   - Converted target variable `diagnosis` to binary (`M = 1`, `B = 0`)  
   - Standardized numerical features using `StandardScaler`  

3. **Modeling**  
   - Implemented **Logistic Regression** for classification  
   - Split dataset into train (80%) and test (20%) sets  
   - Trained the model and predicted tumor classes on new data  

4. **Evaluation**  
   - Metrics: Accuracy, Confusion Matrix  
   - Training Accuracy: ~95%  
   - Testing Accuracy: ~94%  
   - Visualized confusion matrix to analyze false positives and false negatives  

5. **Prediction Function**  
   - Built a `predict_input` function to classify **new tumor samples** as benign or malignant  

## 📈 Results
- Training Accuracy: ~95%  
- Testing Accuracy: ~94%  
- Confusion Matrix:[[70  1]
                    [2 41]]
- Key features influencing prediction: **radius, perimeter, area, concave points**  
- Model successfully classifies breast cancer tumors with high accuracy  

## 📝 Conclusion
This project demonstrates how **Machine Learning classification models** can be applied to medical diagnostics, specifically for **early detection of breast cancer**.  
It can be extended using more advanced algorithms (Random Forest, SVM, XGBoost) or a **web app interface** for practical usage.
