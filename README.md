# Data-Integrity-Tracker

A lightweight data discrepancy tracker built in Python using Google Colab. It compares two datasets (e.g., client records) and generates an audit-friendly report of mismatches and missing entries.

**Repository Structure:**

Data_Integrity_Tracker/

/- Compare data to generate report    - Create Compare data to generate report (raw python code)

/- Data Discrepancy code python.ipynb - Main code (python notebook file) 

/- Dummy Data Frame creation          - Create Dummy Data Frame creation (raw python code)

/- Export data                        - Create Export data (raw python code)

/- Visualization (optional)           - Charts (raw python code)

/- first discrepancy_report.xlsx      - Output file (excel sheet)

# Use Case

Simulates client data verification scenarios like:
- KYC/AML data compliance
- Financial audit preparation
- Customer record consistency checks

# Features

- Detect mismatches in client information (Name, Email, Phone)
- Identify missing or extra entries across datasets
- Generate a discrepancy report as an Excel file
- Visual summary with bar charts of discrepancies

# Technologies Used

- Python (Pandas, NumPy)
- Google Colab (for quick deployment)
- Matplotlib (for charting)
- ExcelWriter (for exporting reports)

# Example Output

- `discrepancy_report.xlsx`: Structured Excel file with 3 sheets:
  - Mismatches
  - Only in Master
  - Only in New

# Sample Chart

Bar chart displaying the count of mismatches vs missing records:

import matplotlib.pyplot as plt

# Count mismatches and unique records
counts = {
    'Mismatches': mismatched.shape[0],
    'Only in Master': only_in_master.shape[0],
    'Only in New': only_in_new.shape[0]
}

# How to Run

1. Open the notebook in Google Colab
2. Upload or generate two CSV files: `master_data.csv` and `new_data.csv`
3. Recommended data set (large) if interested - https://www.kaggle.com/datasets/shwetabh123/mall-customers and name it `master_data.csv` , divide this data set by manually entering some mistakes.
4. Run the comparison script
5. Download `discrepancy_report.xlsx`

# Sample Dataset

Compares a master customer list vs an updated version with intentional errors to simulate real-world scenarios.

**Rights and Usage:**

All reports, documentation, and related artifacts are the intellectual property of Ajmal M S.

Shared resources are provided solely as a record of my involvement, competencies, and learning outcomes.

No content from this repository may be copied, altered, shared, or reused without explicit permission.

© Ajmal M S, 2025
