📌 Loan Status Prediction using Support Vector Machine (SVM)


This project builds a Machine Learning model to predict whether a loan application will be Approved or Not Approved based on applicant demographic and financial details.

The objective is to help financial institutions automate loan approval decisions using data-driven insights.

🛠 Technologies Used

* Python

* NumPy

* Pandas

* Seaborn

* Matplotlib

* Scikit-learn

* Support Vector Machine (SVM)

📊 Project Workflow

1) Data Collection & Loading

2) Data Cleaning and Missing Value Handling

3) Categorical Feature Encoding

4) Exploratory Data Analysis (EDA)

5) Train-Test Split

6) Model Training using SVM

7) Model Evaluation

8) Predictive System Implementation

🤖 Model Details

Algorithm Used: Support Vector Machine (SVM)

Why SVM?

Effective for binary classification problems

Works well in high-dimensional feature spaces

Robust against overfitting

Suitable for structured tabular data

📈 Model Performance

Training Accuracy: 79.86%

Testing Accuracy: 83.33%

The slightly higher test accuracy indicates good generalization on unseen data.

🔍 Model Evaluation
Confusion Matrix
[[9 6]
 [ 2 31]]
Interpretation

Correctly classified 31 approved loans

Correctly classified 9 rejected loans

High recall (94%) for approved loans

Overall F1-score: 0.83

The model performs strongly in identifying eligible applicants, which is critical for financial approval systems.

Classification Report
              precision    recall  f1-score   support

           0       0.82      0.60      0.69        15
           1       0.84      0.94      0.89        33

    accuracy                           0.83        48
   macro avg       0.83      0.77      0.79        48
weighted avg       0.83      0.83      0.83        48
🔮 Predictive System

The project includes two modular functions:

preprocess_input_data()
Handles feature encoding and ensures input consistency.

predict_loan_status()
Takes applicant details and returns:

✅ Approved

❌ Not Approved

Example Usage
prediction = predict_loan_status(
    'Female', 'No', '2',
    'Not Graduate', 'No', 3000,
    0.0, 80.0, 180.0,
    0.0, 'Rural'
)

print("Predicted Loan Status:", prediction)

📦 Installation

Install required dependencies:

pip install numpy pandas seaborn matplotlib scikit-learn
📁 Dataset

The project uses a dataset named:

train.csv

Ensure the dataset path is correctly specified in the notebook before execution.

🔥 Future Improvements

Hyperparameter tuning using GridSearchCV

Cross-validation implementation

Model comparison (Logistic Regression, Random Forest)

Adding probability confidence scores

Deployment using Streamlit or Flask

🎯 Conclusion

This project demonstrates a complete end-to-end machine learning pipeline for loan approval prediction.

With 83.33% test accuracy, the SVM model shows strong generalization and reliable performance for financial classification tasks.
