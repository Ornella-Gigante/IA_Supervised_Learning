Here’s a detailed README for this cardiovascular disease prediction project, incorporating insights from the Jupyter notebook analysis:

---

# 🩺 Cardiovascular Disease Prediction Project  
*By Ornella Sofía Gigante*  

## 📌 Project Overview  
This project aims to predict cardiovascular diseases using patient clinical data. Two machine learning models (Decision Tree and Gaussian Naive Bayes) were implemented and compared for binary classification (disease present/absent).  

---

## 🔍 Dataset  
**Key Features Analyzed**:  
- Age  
- Gender (1 = male)  
- Chest pain type (0-3 scale)  
- Resting blood pressure (mmHg)  
- Serum cholesterol (mg/dl)  
- Fasting blood sugar  
- Resting electrocardiogram results  
- Maximum heart rate  
- Exercise-induced angina  
- ST depression (oldpeak)  
- Slope of peak exercise ST segment  
- Number of major vessels  

**Target Variable**:  
- `target` (1 = disease detected, 0 = no disease)  

---

## 🤖 Models Used  
### 🌳 Decision Tree Classifier  
- Achieved **71.15% accuracy**  
- Advantages: Simple interpretation, handles non-linear relationships  

### 🧪 Gaussian Naive Bayes  
- Achieved **70.49% accuracy**  
- Advantages: Fast computation, works well with small datasets  

---

## 📊 Key Results  
| Metric          | Decision Tree | Naive Bayes |
|-----------------|---------------|-------------|
| **Accuracy**    | 71.15%        | 70.49%      |  

Both models showed similar performance, suggesting room for improvement through:  
- Feature engineering  
- Hyperparameter tuning  
- Larger/more balanced datasets  

---

## 🛠️ How to Run  
1. **Dependencies**:  
   ```python
   pandas==1.5.3
   numpy==1.24.3
   scikit-learn==1.2.2
   jupyter==1.0.0
   ```

2. **Execution Steps**:  
   ```bash
   # Clone repository
   git clone https://github.com/username/cardio-prediction.git
   
   # Launch Jupyter notebook
   jupyter notebook Ornella_Gigante_lab4.ipynb
   ```

---

## 🚀 Future Improvements  
- 🔧 Experiment with deeper tree structures and pruning  
- 🤖 Test ensemble methods (Random Forest, XGBoost)  
- 🧬 Incorporate additional medical biomarkers  
- 📈 Implement cross-validation for robust evaluation  
- ⚖️ Address potential class imbalance  

*Developed using Python 3.9 and Jupyter Lab environment.*  

--- 

This project demonstrates foundational ML workflow implementation for healthcare diagnostics, with potential real-world applications in early disease detection.

