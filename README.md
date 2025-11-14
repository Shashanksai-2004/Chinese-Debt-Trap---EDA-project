📘 China Debt Dataset – Exploratory Data Analysis (EDA)

A complete exploratory data analysis on China’s global lending dataset.
This project focuses on uncovering trends in international debt distribution, borrower types, sensitive territory overlaps, funded sectors, and year-wise funding patterns.
The notebook includes data cleaning, preprocessing, feature engineering, and extensive visual analysis.

📑 Table of Contents

Project Overview

Dataset Description

Data Cleaning & Preprocessing

Exploratory Data Analysis

Univariate Analysis

Bivariate Analysis

Key Insights

Tech Stack

Project Structure

How to Run the Project

Conclusion

📌 Project Overview

This project performs an in-depth Exploratory Data Analysis (EDA) on an international debt dataset, with an emphasis on China’s global lending.
The analysis identifies:

Countries receiving the highest loans

Sector-wise investment patterns

Borrower-type behavior

Yearly investment trends

Overlaps with sensitive territories (Indigenous, Critical, Protected)

Multiple visualizations help uncover patterns, anomalies, and significant relationships within the dataset.

📂 Dataset Description

The dataset includes:

AMOUNT of loan (in M/B, cleaned to numeric)

LENDER names (multiple values per entry)

BORROWER TYPE

COUNTRY

SECTOR funded by China

YEAR of loan issuance

SENSITIVE TERRITORY OVERLAP flags

Other categorical and numeric features

🧹 Data Cleaning & Preprocessing

The raw data required significant preprocessing:

✔ Missing Value Handling

Dropped incomplete rows

Verified data consistency post-cleaning

✔ AMOUNT Cleaning

Converted strings like:

$50M → 50

$2B → 2000
Using custom conversion logic.

✔ Multi-Valued Columns

Columns like LENDER and SENSITIVE_TERRITORY_OVERLAP contained multiple values separated by commas/newlines.

Extracted unique values

Created binary indicator columns for each label

✔ Sector Standardization

Inconsistent sector names (typos, spacing issues) were fixed through value replacement.

✔ New Features

STO_Indigenous

STO_Critical

STO_Protected
(For sensitive territory categories)

📊 Exploratory Data Analysis
🔹 Univariate Analysis

Distribution of Loan Amounts — Boxplots, histograms

Year-wise Loan Frequency — Countplots

Sector Distribution — Bar charts

Borrower Type Analysis

Sensitive Territory Overlap Frequency

🔸 Bivariate Analysis

Year vs Amount trends

Top & bottom borrowing countries (bar charts & horizontal bars)

Sector-wise funding by country

Borrower type vs loan amount

Impact of sensitive territories on loan amounts

Correlation exploration through grouped summaries

⭐ Key Insights

A small group of countries receives the majority of China's debt funding.

Infrastructure, energy, and multi-sector development dominate sector-wise funding.

Year-wise funding shows clear peaks corresponding to major investment cycles.

Borrower types like sovereign borrowers receive significantly larger loans.

Many projects overlap with indigenous, critical, or protected territories.

Lender data shows a wide variety of financial institutions contributing to funding.

🛠 Tech Stack

Python

Pandas

NumPy

Matplotlib

Seaborn

Jupyter Notebook

🏁 Conclusion

This project provides a complete exploratory analysis of China's international debt dataset, highlighting financial trends, geopolitical indicators, sector behavior, and borrower patterns.
It serves as a strong foundation for further predictive modeling, dashboard creation, or policy analysis.
