# 📊 LERS Enrolment Data Extraction & Conversion Script

T-SQL query for enrolment data extraction from Student Information System, in CSV format. Python script is used for converting data in CSV format into custom XML format for DCaR upload. 

---

## 🔍 Overview

The current solution for LERS data reporting is outdated and no longer maintainable. The solution provided here uses SQL for data extraction and allows for future modifications to extraction conditions when needed. Python script converts CSV extract into custom XML extract while maintaining the required parent and child relationship in the XML data structure. 

---

## 🚀 Features

- Enrolment data extraction with SQL, can be custom modified each year based on reporting requirement changes. 
- Conversion of CSV data into XML data, maintains the parent/child relationship required for DCaR reporting.

---

## 🛠️ Tech Stack

**Languages:** 
-SQL, Python

**Libraries:** 
- csv — reading and writing CSV files
- xml.etree.ElementTree — XML parsing and tree-based data extraction
- xml.dom.minidom — XML formatting and pretty-printing
- lxml — advanced XML parsing, XPath, and schema validation
- difflib (unified_diff) — line-by-line file comparison and diff generation

---

## ▶️ User Instructions

### 1️⃣ Clone the repository
git clone https://github.com/guochuanyong/LERS-Enrolment-Data-Reporting.git

### 2️⃣ Install Python dependencies
pip install lxml

### 3️⃣ Run the data extraction script
'LERS Data Extraction Query.sql'

### 4️⃣ Convert extracted CSV file into XML with Python script
In the Jupyter file 'DCaR LERS Submission - Custom CSV to XML Converter.ipynb', modify the line 'with open("data_extract.csv", mode="r") as file:' to match your file name. 

### 5️⃣ Upload XML data to DCaR
Upload the generated XML data file in the same folder to DCaR. 

