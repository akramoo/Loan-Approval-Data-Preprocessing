# Loan Approval Data Preprocessing

This repository contains a Python script that preprocesses the **Loan-Approval** dataset, a fictional dataset of loan applicants, as part of a data preparation exercise. The script implements a full preprocessing pipeline, including handling missing data, encoding categorical variables, treating outliers, applying transformations, standardizing features, and performing feature selection. A hot-fix is included to convert any `True`/`False` columns to numeric values (`1`/`0`) for machine learning compatibility.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Preprocessing Steps](#preprocessing-steps)
- [Hot-Fix for True/False Columns](#hot-fix-for-truefalse-columns)
- [Dependencies](#dependencies)
- [File Structure](#file-structure)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
The goal of this project is to preprocess the **Loan-Approval** dataset to prepare it for machine learning tasks. The preprocessing follows the requirements of **Exercice 02** from a data preparation assignment, which includes:
- Loading and inspecting the dataset.
- Handling incorrect entries and missing data using both Pandas and Scikit-learn.
- Encoding categorical variables (binary, ordinal, and nominal).
- Detecting and capping outliers.
- Applying transformations to reduce skewness.
- Standardizing numerical features.
- Performing feature selection using Pearson correlation and Chi-squared tests.
- Splitting data into features (`X`) and target (`y`).
- Converting `True`/`False` columns to numeric format.

The script is designed to be modular, well-commented, and reusable for similar datasets.

## Dataset
The **Loan-Approval** dataset contains 600 observations and 14 attributes related to loan applicants. It is provided in CSV format (`Loan-Approval.csv`). Key attributes include:
- `Loan_ID`: Unique identifier.
- `Gender`: Male/Female.
- `Married`: Yes/No.
- `Dependents`: Number of dependents (0, 1, 2, 3+).
- `Education`: Graduate/Not Graduate.
- `Self_Employed`: Yes/No.
- `ApplicantIncome`: Applicant’s income.
- `CoapplicantIncome`: Co-applicant’s income.
- `LoanAmount`: Loan amount requested.
- `Loan_Amount_Term`: Loan term in months.
- `Credit_History`: Credit history (0 or 1).
- `Risk`: Credit risk (Yes/No).
- `Property_Area`: Urban/Semiurban/Rural.
- `Loan_Status`: Loan approval status (Y/N).

*Note*: The dataset is not included in this repository due to potential licensing restrictions. Users must provide their own `Loan-Approval.csv` file.

## Features
- **Comprehensive Preprocessing**: Handles all aspects of data preparation required for machine learning.
- **Dual Imputation Methods**: Implements missing data handling with both Pandas and Scikit-learn.
- **Hot-Fix for Booleans**: Converts `True`/`False` columns (e.g., from one-hot encoding) to `1`/`0`.
- **Feature Selection**: Uses statistical tests (Pearson correlation, Chi-squared) to identify significant features.
- **Well-Documented Code**: Includes detailed comments explaining each step.
- **Reproducible**: Designed to work with the provided dataset structure and easily adaptable to similar datasets.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/loan-approval-data-preprocessing.git
   cd loan-approval-data-preprocessing
