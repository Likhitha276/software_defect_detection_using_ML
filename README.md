# Software Defect Prediction

## 📌 Introduction
Software Defect Prediction is a critical aspect of software engineering that aims to identify potential defects before deployment.  
This project leverages **machine learning techniques** to predict defects based on historical software metrics, improving quality and reducing maintenance costs.

## 🎯 Motivation
- Enhance software quality
- Reduce maintenance costs
- Improve customer satisfaction
- Automate defect detection with data-driven approaches

## 📂 Dataset
- **Size**: 10,885 entries, 22 features  
- **Target variable**: `defects`  
- Features include software metrics such as `loc`, `v(g)`, `lOCode`, etc.  
- Dataset used: `Software Defect Prediction.csv`

## 🔬 Related Work
1. **Software Defects Prediction Using Machine Learning**  
   *Mitt Shah, Nandit Pujara* – Found Neural Networks and Gradient Boosting to perform best on NASA datasets.
   
2. **Software Defect Prediction System Based on Decision Tree Algorithm**  
   *Umar Abdullahi Muhammad* – Focuses on decision trees, hyperparameter tuning, and computational efficiency.

3. **Survey on Software Defect Prediction Using Machine Learning Techniques**  
   *Pooja Paramshetti, D. A. Phalke* – A review of machine learning methods to improve quality and reduce testing costs.

## ⚙️ Methodology
1. **Data Loading and Inspection**  
   - Libraries: `NumPy`, `pandas`, `scikit-learn`  
   - Handle missing values  

2. **Model Training & Evaluation**  
   - Classifier: **Random Forest**  
   - Hyperparameter tuning: **GridSearchCV** with cross-validation  
   - Evaluation Metric: **F1 Macro Score**

3. **Feature Importance**  
   - Bar plot visualization to show the contribution of each feature.

## 📊 Results
- Best hyperparameters obtained via GridSearchCV
- Performance evaluated using **F1 score** and classification report

## ⚠️ Threats to Validity
- Dataset bias  
- Generalization issues across different software projects  
- Limited exploration of other ML models  

## ✅ Conclusion
- Random Forest classifier shows strong predictive power for software defect detection.
- The project demonstrates the potential of machine learning to improve software reliability.

## 🔮 Future Scope
- Explore deep learning models for better accuracy  
- Apply ensemble techniques for robust prediction  
- Use larger and more diverse datasets  
- Integrate predictions into CI/CD pipelines for real-time defect monitoring

---

## 🚀 How to Run
```bash
# Clone repository
git clone <repo-url>
cd software-defect-prediction

# Install dependencies
pip install -r requirements.txt

# Run the model training
python train_model.py
