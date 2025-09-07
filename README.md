Prediction of Loan Defaulters
📌 Project Overview

This project focuses on predicting loan defaulters using customer transaction and profile data. Financial institutions often face challenges in identifying high-risk customers, which can lead to significant losses. By leveraging machine learning, this project aims to build a predictive model that classifies customers into defaulter or non-defaulter, enabling smarter credit decisions.

The dataset includes both transactional and demographic information, providing a holistic view of customer behavior. Since the data was imbalanced, different resampling techniques were tested. Ultimately, oversampling was chosen as it provided better performance compared to undersampling, ensuring enough records for the model to learn effectively.

📂 Dataset Description

The dataset consists of customer transaction details along with demographic and financial attributes.

Columns include:

transaction_id – Unique identifier for each transaction

customer_id – Unique identifier for each customer

customer_name – Name of the customer

gender – Gender of the customer

age – Age of the customer

location – Customer’s residential or transactional location

transaction_date – Date of the transaction

purchase_amount – Total purchase amount of the transaction

down_payment – Initial payment made by the customer

installment_amount – Amount to be paid in each installment

installments – Total number of installments for repayment

payment_status – Current status of payments (on-time, delayed, etc.)

product_category – Category of the purchased product

merchant_name – Name of the merchant/vendor

customer_income – Income level of the customer

credit_score – Credit score associated with the customer

late_payments – Number of late payments made by the customer

account_created – Date when the customer’s account was created

fraud_flag – Target variable (1 = default/fraud, 0 = non-default)

⚙️ Methodology

Data Preprocessing – Cleaning, handling missing values, encoding categorical features, and scaling.

Exploratory Data Analysis (EDA) – Understanding feature distributions, correlations, and patterns.

Handling Imbalanced Data –

Tried undersampling (did not provide enough records).

Implemented oversampling, which performed better given low correlation between features.

Model Building – Applied machine learning classifiers to predict defaulters.

Evaluation – Models were evaluated using precision, recall, F1-score, and accuracy.

📊 Results

Achieved an overall accuracy of 97%.

Class 1 (Defaulters): Recall = 1.00, meaning all defaulters were successfully identified.

Class 0 (Non-defaulters): Precision = 1.00, meaning non-defaulters were almost always predicted correctly.

This balance between precision and recall ensures that the model is reliable for practical use in financial risk assessment.

🎯 Objective

To develop a machine learning solution that accurately predicts loan defaulters, helping financial institutions reduce risks, optimize lending, and improve customer screening.
