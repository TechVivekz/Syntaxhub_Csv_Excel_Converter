# ✨ CSV to Excel Converter 🚀

> A powerful and beginner-friendly Python tool to convert CSV files into Excel spreadsheets with automatic data cleaning and preprocessing.

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python">
  <img src="https://img.shields.io/badge/Pandas-Data%20Processing-green?style=for-the-badge&logo=pandas">
  <img src="https://img.shields.io/badge/OpenPyXL-Excel-orange?style=for-the-badge">
  <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge">
</p>

---

# 📌 Overview

This project is a command-line utility built using Python that converts CSV files into Excel files while automatically:

✅ Cleaning column names  
✅ Handling missing values  
✅ Parsing date columns  
✅ Renaming columns  
✅ Creating output directories  
✅ Logging every operation  

Perfect for:
- 📊 Data Cleaning
- 📁 File Conversion
- 🧹 Dataset Preprocessing
- 🎓 Student Projects
- 💼 Automation Tasks

---

# 🌟 Features

## 🔹 CSV to Excel Conversion
Convert `.csv` files into `.xlsx` files instantly.

---

## 🔹 Automatic Column Cleaning

The tool automatically:
- Converts column names to lowercase
- Removes extra spaces
- Replaces spaces with underscores

### Example

```text
" User Name " → "user_name"
```

---

## 🔹 Missing Value Handling

| Data Type | Replacement |
|-----------|-------------|
| Numeric | `0` |
| String/Object | `"Unknown"` |

---

## 🔹 Automatic Date Parsing

The program attempts to detect and convert date columns automatically.

Example:

```text
2025-05-12 → Datetime Format
```

---

## 🔹 Column Renaming Support

Rename columns directly from the command line.

### Example

```bash
python converter.py -i data.csv -o output.xlsx -r "name=full_name,age=user_age"
```

---

## 🔹 Logging System

The project includes detailed logging for:
- File Reading
- Data Cleaning
- Excel Export
- Error Handling

### Example Logs

```text
INFO - Reading CSV file...
INFO - Cleaning column names...
INFO - Exporting to Excel...
INFO - Conversion successful!
```

---

# 🛠️ Libraries Used

| Library | Purpose |
|---------|---------|
| `pandas` | Reading and processing CSV data |
| `openpyxl` | Writing Excel `.xlsx` files |
| `argparse` | Handling command-line arguments |
| `logging` | Logging messages and errors |
| `os` | File and directory operations |

---

# 🧰 Technologies Used

| Technology | Purpose |
|------------|---------|
| Python 🐍 | Core Programming |
| pandas 📊 | Data Processing |
| openpyxl 📑 | Excel Export |

---

# 📂 Project Structure

```text
📁 csv-to-excel-converter
│
├── 📄 converter.py
├── 📄 input.csv
├── 📄 output.xlsx
├── 📄 README.md
└── 📄 LICENSE
```

---

# ⚡ Installation

## Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/csv-to-excel-converter.git
```

---

## Step 2: Navigate to Project Folder

```bash
cd csv-to-excel-converter
```

---

## Step 3: Install Dependencies

```bash
pip install pandas openpyxl
```

---

# ▶️ How to Run the Code

## 🔹 Basic Example

```bash
python converter.py -i input.csv -o output.xlsx
```

### Explanation

| Command Part | Meaning |
|-------------|---------|
| `python` | Runs the Python interpreter |
| `converter.py` | Main Python file |
| `-i input.csv` | Input CSV file |
| `-o output.xlsx` | Output Excel file |

---

## 🔹 Example with Column Renaming

```bash
python converter.py -i employees.csv -o employees.xlsx -r "name=full_name,salary=monthly_salary"
```

---

## 🔹 Example Output in Terminal

```text
2026-05-12 10:30:10 - INFO - Reading CSV file...
2026-05-12 10:30:11 - INFO - Cleaning column names...
2026-05-12 10:30:12 - INFO - Handling missing values...
2026-05-12 10:30:13 - INFO - Parsing date columns...
2026-05-12 10:30:14 - INFO - Exporting to Excel...
2026-05-12 10:30:15 - INFO - Conversion successful!
```

---

# 🧪 Example

## 📥 Input CSV

| Name | Age | Joining Date |
|------|-----|---------------|
| Bibek | 21 | 2025-01-01 |
| Ravi |  | 2025-02-10 |

---

## 📤 Output Excel

| full_name | user_age | joining_date |
|-----------|----------|---------------|
| Bibek | 21 | 2025-01-01 |
| Ravi | 0 | 2025-02-10 |

---

# ❌ Error Handling

The application can handle:

✅ Missing files  
✅ Empty CSV files  
✅ Invalid CSV formats  
✅ Unexpected runtime errors  

---

# 👨‍💻 About the Developer

## Bibekanand Sing

This project was created to simplify CSV to Excel conversion while learning real-world data preprocessing techniques using Python.




