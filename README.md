# Chinese-Debt-Trap---EDA-project

📌 China Debt Dataset – Exploratory Data Analysis (EDA)

This project focuses on performing an in-depth Exploratory Data Analysis (EDA) on an international debt dataset, with a specific emphasis on China’s lending patterns, borrower characteristics, sensitive territories, and sector-wise distribution of debt. The aim of the analysis is to clean, transform, visualize, and extract insights that help understand global debt dependencies and financial exposure.

🔍 Project Overview

The dataset contains details on:

Loan amount (in millions/billions)

Lending institutions

Borrower type

Country receiving the loan

Sensitive territory overlaps (Indigenous, Critical, Protected areas)

Sector in which the loan was issued

Year-wise distribution of debt

This analysis transforms raw financial data into meaningful insights using Python, Pandas, and Seaborn/Matplotlib visualizations.

🧼 Data Cleaning & Preprocessing

Key preprocessing steps included:

Handling missing values and removing incomplete records

Cleaning AMOUNT by converting values from strings (e.g., "$50M", "$2B") into numerically consistent units

Splitting multi-value columns such as LENDER and SENSITIVE_TERRITORY_OVERLAP into separate binary indicator variables

Standardizing inconsistent sector names and fixing formatting errors

Converting categorical features into analyzable forms for uni-variate and bi-variate visual analysis

📊 Exploratory Data Analysis (EDA)
Univariate Analysis

Distribution plots for loan amounts, revealing large right-skew due to high-value loans

Year-wise loan frequency and trends

Sector-wise loan count to identify commonly funded sectors

Borrower type distribution

Sensitive territory overlaps and frequency analysis

Bivariate Analysis

Relationship between loan amount vs year

Top 20 countries by total borrowing

Borrower-type segmentation of loans

Sector-wise debt analysis per country

Impact of sensitive territory categories (Indigenous / Critical / Protected) on loan allocation

Sector and borrower type cross-analysis

Visualizations include boxplots, countplots, histograms, bar charts (vertical & horizontal), and grouped bar graphs.

📈 Key Insights Extracted

China issues significantly large amounts of debt to a small set of high-dependence countries.

Certain sectors—especially infrastructure, multi-sector development, and energy—receive the highest share of loans.

Multi-borrower loans and sovereign borrowers dominate the dataset.

Sensitive territory overlaps (Indigenous / Protected / Critical) are present in multiple projects, indicating geopolitical and environmental considerations.

Loan amounts show clear growth trends across specific years, with notable spikes indicating major project funding cycles.

🛠️ Tech Stack Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Jupyter Notebook

📁 Project Structure
├── china_debt.csv
├── EDA-China-Debt.ipynb
└── README.md
