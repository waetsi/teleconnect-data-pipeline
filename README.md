# Teleconnect Data Pipeline

This project demonstrates an end-to-end **data engineering pipeline** using Python.

It simulates telecom Call Detail Records (CDR) processing, including:
- data extraction
- quality assessment
- cleaning and transformation
- business rule validation
- feature engineering
- data loading to CSV and SQLite database

## 📁 Dataset
- `teleconnect_cdr_data.csv` (raw input)
- `cdr_cleaned.csv` (processed output)

## 🛠️ Tech Stack
- Python
- pandas
- numpy
- SQLAlchemy
- SQLite
- VS Code
- GitHub

## ⚙️ Pipeline Steps

1. **Data Extraction**
   - Read CSV with enforced data types

2. **Data Quality Assessment**
   - Missing values
   - Duplicates
   - Inconsistent categories

3. **Data Cleaning & Transformation**
   - Drop unusable records
   - Fill missing values
   - Standardise text and booleans
   - Convert timestamps

4. **Data Validation (Business Rules)**
   - Signal strength range validation
   - Phone number validation

5. **Feature Engineering**
   - Signal quality classification (Good/Fair/Poor)
   - Time-based features (hour, day, month)
   - Customer revenue aggregation

6. **Data Loading**
   - Export cleaned data to CSV
   - Load final dataset into SQLite database

## ▶️ How to Run

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
python pipeline.ipynb


## 🧪 Environment
- Python 3.8
- Virtual environment (.venv)
- Jupyter Notebook (ipykernel)
- Windows PowerShell

