# Data-Preprocessing-for-Data-Analysis
Here's a professional README file for your GitHub repository:

---

# Lending Company Data Cleaning

This repository contains the code and data for cleaning and preparing the `Lending-company.csv` dataset for further analysis. The dataset includes information about loans, customers, and loan statuses. The cleaning process involves several steps to ensure the data is ready for analysis.

## Table of Contents

- Introduction
- Dataset
- Data Cleaning Steps
- Installation
- Usage
- Contributing
- License
- Contact

## Introduction

The goal of this project is to clean and preprocess the `Lending-company.csv` dataset. The dataset contains various columns related to loans, customers, and their statuses. The cleaning process includes handling missing values, converting categorical data to numerical data, and extracting useful information from date columns.

## Dataset

The dataset `Lending-company.csv` includes the following columns:

- `LoanID`
- `StringID`
- `Product`
- `CustomerGender`
- `Location`
- `Region`
- `TotalPrice`
- `StartDate`
- `Deposit`
- `DailyRate`
- `TotalDaysYr`
- `AmtPaid36`
- `AmtPaid60`
- `AmtPaid360`
- `LoanStatus`

## Data Cleaning Steps

The following steps were performed to clean the dataset:

1. **Dropped the `LoanID` and `StringID` columns.**
2. **Mapped the `Product` categories to numeric data:**
   - Product A to 0
   - Product B to 1
   - Products C, D, E, and F to 2
3. **Replaced `NotSpecified` in the `CustomerGender` column with the mode of the column.**
4. **Extracted the numeric values from the `Location` and `Region` columns and converted them to integers.**
5. **Filled missing values in the `TotalPrice` column with the column mean.**
6. **Dropped all rows with missing `StartDate` values and extracted the month and weekday as separate columns.**
7. **Dropped the `StartDate` column.**
8. **Examined the `TotalDaysYr` column.**
9. **Dropped all rows with missing `LoanStatus` values and where the status is `Blocked`. Mapped `Active` to 0 and `Finished Payment` to 1.**

## Installation

To run the data cleaning script, you need to have Python installed. You can install the required packages using pip:

```bash
pip install pandas numpy
```

## Usage

1. Clone the repository:
```bash
git clone https://github.com/yourusername/lending-company-data-cleaning.git
```

2. Navigate to the project directory:
```bash
cd lending-company-data-cleaning
```

3. Run the data cleaning script:
```bash
python data_cleaning.py
```

The cleaned data will be saved to a new file named `Lending-company-cleaned.csv`.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.

