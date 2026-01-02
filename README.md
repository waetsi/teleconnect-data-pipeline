# Teleconnect Data Pipeline

This project demonstrates an end-to-end **data engineering pipeline** using Python.

It simulates telecom Call Detail Records (CDR) processing, covering the full lifecycle from raw data ingestion to cleaned, validated, and analytics-ready outputs.

---

## 📁 Dataset
- `teleconnect_cdr_data.csv` — raw input dataset
- `cdr_cleaned.csv` — processed and cleaned output

---

## 🛠️ Tech Stack
- Python
- pandas
- numpy
- SQLAlchemy
- SQLite
- Jupyter Notebook
- VS Code
- GitHub

---

## ⚙️ Pipeline Steps

### 1. Data Extraction
- Read CSV with enforced data types to preserve identifiers (e.g. phone numbers)

### 2. Data Quality Assessment
- Missing values
- Duplicate records
- Inconsistent categorical values

### 3. Data Cleaning & Transformation
- Drop unusable records
- Fill missing numerical values
- Standardise text fields and boolean values
- Convert timestamps to datetime

### 4. Data Validation (Business Rules)
- Validate signal strength ranges
- Validate phone number formats

### 5. Feature Engineering
- Signal quality classification (Good / Fair / Poor)
- Time-based features (hour, day of week, month)
- Customer revenue aggregation

### 6. Data Loading
- Export cleaned data to CSV
- Load final dataset into a SQLite database

---
“Things I struggled with during setup”:

virtual environments
PowerShell vs VS Code
ipykernel confusion
connecting to github


## ▶️ How to Run

### 1. Create and activate a virtual environment

```bash
python -m venv .venv
# Windows
.\.venv\Scripts\Activate.ps1
