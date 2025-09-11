**IBM-Telco-Customer-Churn**

**Executive Summary**
This project predicts customer churn using the IBM Telco dataset. Churn is when customers discontinue a service, and preventing it is crucial since retaining existing customers is far cheaper than acquiring new ones. Predicting customer churn using the IBM Telco dataset with Logistic Regression and Random Forest. Includes data cleaning, leakage prevention, imbalance handling, and model evaluation. Provides business insights on contracts, tenure, services, and charges to improve customer retention.

**Goals**
Clean and preprocess customer data (handle missing values, remove leakage).
Explore churn behavior with EDA and visualizations.
Build and compare Logistic Regression (baseline) and Random Forest (advanced).
Evaluate models using Accuracy, F1, Recall, Precision, and ROC AUC.
Translate results into business recommendations.

**📊 Key Results**
Model	Accuracy	Precision (Churn)	Recall (Churn)	F1 (Churn)	ROC AUC
Logistic Regression	0.70	0.45	0.50	0.47	0.72
Random Forest	0.78	0.59	0.60	0.60	0.84


**💡 Business Insights**
Month-to-month contracts → Highest churn → Offer incentives for annual plans.
Short tenure customers → Need onboarding and loyalty programs.
Bundled services (e.g., online security, tech support) → Lower churn.
High-charge customers → Monitor and provide targeted retention offers.


🛠️ Installation & Setup
# 🔹 Clone the repository
git clone https://github.com/Whitewolf258/ibm-churn-prediction.git
cd ibm-churn-prediction

# 🔹 (Optional) Create a virtual environment
python -m venv venv
# Activate it:
# Windows:
venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate

# 🔹 Install dependencies
pip install -r requirements.txt

# 🔹 Launch Jupyter Notebook
jupyter notebook

📊 Exploratory Data Analysis (EDA)

Key findings from EDA:

Customers on month-to-month contracts churned the most.

Tenure strongly correlates with churn — short-tenure customers are at higher risk.

Lack of online security and technical support increases churn probability.

High total charges without added services drive dissatisfaction.

🤖 Modeling Approach

Logistic Regression → Baseline, interpretable.

Random Forest → More powerful, handles non-linear patterns.

Imbalance Handling → Applied class weights and SMOTE.

📈 Model Results
Logistic Regression

Accuracy: 70%

Precision (Churn): 0.45

Recall (Churn): 0.50

F1 (Churn): 0.47

ROC AUC: 0.72

➡️ Captures ~50% of churners but misses half.

Random Forest

Accuracy: 78%

Precision (Churn): 0.59

Recall (Churn): 0.60

F1 (Churn): 0.60

ROC AUC: 0.84

➡️ Captures ~60% of churners and offers stronger predictive performance overall.

💡 Business Recommendations
Provide discounts or perks to month-to-month customers to push annual contracts.

Introduce early loyalty rewards for short-tenure customers.

Encourage adoption of bundled services (security, tech support).

Track high-charge customers for dissatisfaction signals and intervene proactively.

🚀 Next Steps

Deploy the model via an API or integrate into a CRM dashboard.

Explore XGBoost/LightGBM for further improvements.

Implement cost-sensitive learning to align retention strategies with ROI.

📜 License

This project is released under the MIT License.

🙋 Author

👤: Satyam Kumar Shivam

LinkedIn: www.linkedin.com/in/satyam-kumar--shivam
