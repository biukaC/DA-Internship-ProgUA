# DA Internship ProgUA
DataAnalysis for IT school

Python pipeline for cleaning CRM export and preparing data for Power BI.

---

## Pipeline

* Parsed all date columns into a datetime format.
* Filled missing values in ‘Created on’ by combine/merge with ‘Modify on’ (see new column ‘Created filled’).
* Removed raws with invalid time (future dates, modified before created, etc.)
* Finded and combined all UTM columns. Duplicates deleted after merging.
* Deleted null-values and low-filled (less then 5% filled) columns.
* Combined columns with similar info (phone, e-mail, notes).
* changed columns types
* filled phones complete type
* merged manager, course_name columns. Duplicates deleted after merging.
* droped raw source columns

---

## Data Cleaning

* remove empty columns
* remove technical columns
* remove raw UTM/referrer/manager/course_name columns after merge

---

## Input

crm_output.csv

---

## Output

cleaned.csv
