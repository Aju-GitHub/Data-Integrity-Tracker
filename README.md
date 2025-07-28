# Data-Integrity-Tracker

1. Data Integrity Tracker

A lightweight data discrepancy tracker built in Python using Google Colab. It compares two datasets (e.g., client records) and generates an audit-friendly report of mismatches and missing entries.

2. Use Case

Simulates client data verification scenarios like:
- KYC/AML data compliance
- Financial audit preparation
- Customer record consistency checks

3. Features

- Detect mismatches in client information (Name, Email, Phone)
- Identify missing or extra entries across datasets
- Generate a discrepancy report as an Excel file
- Visual summary with bar charts of discrepancies

4. Technologies Used

- Python (Pandas, NumPy)
- Google Colab (for quick deployment)
- Matplotlib (for charting)
- ExcelWriter (for exporting reports)

5. Example Output

- `discrepancy_report.xlsx`: Structured Excel file with 3 sheets:
  - Mismatches
  - Only in Master
  - Only in New

6. Sample Chart

Bar chart displaying the count of mismatches vs missing records:

import matplotlib.pyplot as plt

# Count mismatches and unique records
counts = {
    'Mismatches': mismatched.shape[0],
    'Only in Master': only_in_master.shape[0],
    'Only in New': only_in_new.shape[0]
}

7. How to Run

1. Open the notebook in Google Colab
2. Upload or generate two CSV files: `master_data.csv` and `new_data.csv`
3. Recommended data set (large) if interested - https://www.kaggle.com/datasets/shwetabh123/mall-customers and name it `master_data.csv` , divide this data set by manually entering some mistakes.
4. Run the comparison script
5. Download `discrepancy_report.xlsx`

8. Sample Dataset

Compares a master customer list vs an updated version with intentional errors to simulate real-world scenarios.

Author

Ajmal M S  
M.Sc. Computer Science (Data Analytics)  
LinkedIn: https://linkedin.com/in/ajmal-m-s
