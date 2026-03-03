# Loan Approval Prediction Project

## 📌 About the Project
This project builds a Machine Learning model to predict whether a loan application will be approved based on applicant and campaign-related details.

The dataset (`loan_detection.csv`) contains demographic and behavioral features such as age, job, education, previous contact history, and campaign information.

A key challenge in this dataset was **class imbalance**, so evaluation focused on F1-score and recall rather than only accuracy.

---

## 🎯 Problem Statement
Banks and financial institutions must make accurate loan approval decisions to reduce financial risk while maintaining growth.

Project objectives:
- Predict loan approval status (Yes/No)
- Handle imbalanced data effectively
- Compare multiple ML models
- Select the best model using appropriate evaluation metrics

---

## ⚙️ Approach
- Data cleaning and preprocessing
- Handling missing values
- Encoding categorical variables
- Addressing class imbalance using class weights
- Train-test split
- Model comparison
- Hyperparameter tuning using `RandomizedSearchCV`

### Models Compared
- Logistic Regression  
- Decision Tree  
- Random Forest  

---

## 🤖 Final Model Selection
Random Forest performed best overall, especially in predicting the minority class.

Although hyperparameter tuning was applied, the baseline Random Forest already delivered strong performance. Therefore, Random Forest was selected as the final model.

---

## 📊 Final Model Performance
- Accuracy: ~85%
- F1-score (Minority Class): ~0.41
- Good balance between precision and recall
- Strong ROC-AUC performance

Since the dataset is imbalanced, more emphasis was placed on detecting minority class cases rather than maximizing accuracy.

---

## 🔍 Feature Importance Insights
Top influential features:
- Age
- Number of campaign contacts
- Previous contact history
- Job type
- Education level

Both demographic and behavioral factors significantly influence loan approval decisions.

---

## 🛠️ Tools & Technologies
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Jupyter Notebook

---

## 🚀 How to Run
1. Clone the repository:
git clone https://github.com/dhaintrybhagyalaxmi/Loan-detection.git⁠�
Copy code

2. Navigate to the folder:
cd Loan-detection
Copy code

3. Install dependencies:
pip install -r requirements.txt
Copy code

4. Run Jupyter Notebook:
jupyter notebook
Copy code

---

## 📚 What I Learned
- Handling imbalanced datasets
- Choosing proper evaluation metrics
- Comparing ML models effectively
- Hyperparameter tuning
- Interpreting feature importance for business insights