📘 Customer Churn Prediction – Bank Dataset

🔍 Objective
The aim of this project is to predict which customers are likely to leave the bank using a classification model. Understanding churn behavior can help banks take preemptive action to retain high-risk customers.

📁 Dataset
Name: Churn_Modelling.csv 
excel file

🛠️ Project Steps
1. Data Cleaning & Preparation
Dropped irrelevant columns: RowNumber, CustomerId, Surname

Checked and handled missing values

2. Feature Encoding
Encoded Gender using Label Encoding

Encoded Geography using One-Hot Encoding (with drop_first=True to avoid multicollinearity)

3. Feature Selection
Features include: CreditScore, Age, Tenure, Balance, NumOfProducts, etc.

Target: Exited

4. Model Training
Used Random Forest Classifier

Train-Test Split: 80% training / 20% testing

5. Evaluation
Metrics: Accuracy, Precision, Recall, F1-Score

Model Accuracy: ~86.6%

Strong performance in identifying non-churners, moderate for churners

6. Feature Importance Analysis
Most influential features:

Age

EstimatedSalary

CreditScore

Balance

NumOfProducts
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/efb15faf-7601-4615-95bd-65df2fbce1c9" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c2373a02-6f13-4c15-af7f-ab985d4989d2" />


🧪 Technologies Used
Python

Pandas, NumPy

Scikit-learn

Matplotlib, Seaborn

Jupyter Notebook

🚀 How to Run
Download the dataset Churn_Modelling.csv.

Open churn_prediction.ipynb in Jupyter Notebook.

Run all cells sequentially.

View performance metrics and feature importance chart.



✅ Conclusion

This project successfully demonstrates a predictive approach to identifying customer churn in a banking context using machine learning. After cleaning and preprocessing the dataset, a Random Forest Classifier was trained and achieved an accuracy of 86.6%.

The analysis revealed that customer age, account balance, salary, and product engagement are the most significant predictors of churn. Specifically, older and less engaged customers with high balances are more likely to leave the bank.

While the model performs well overall—especially at identifying customers who stay—its ability to predict churners could be improved further through advanced techniques like model tuning, ensemble methods (e.g., XGBoost), or resampling imbalanced data.

This project serves as a foundational step toward a data-driven customer retention strategy, enabling banks to proactively engage with high-risk clients and reduce churn rates.


