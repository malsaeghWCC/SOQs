# 🎓 SOQ Calendar Automation

Automate the generation of **Student Opinion Questionnaire (SOQ)** calendar dates for each academic term — directly from the BlueCourses export data.  
This repository includes scripts and documentation to streamline how WCC’s CiTL prepares official SOQ Date documents each semester.

---

## 📘 Overview

This project extracts, organizes, and formats **Part of Term (POT)** data and corresponding **evaluation (SOQ)** dates.  
It produces:
- A clean **Excel file** summarizing all key dates per semester  
- A **formatted Word document** ready for publication on faculty and dean dashboards

---

## ⚙️ Files Included

| File | Description |
|------|--------------|
| `_Codetoextract.ipynb` | Jupyter Notebook that extracts and aggregates SOQ data from `BlueCourses.csv`. |
| `NEWSOQCalender.xlsx` | Example Excel output from the notebook. |

---

## 🧠 How It Works

### Steps: Data Extraction (`_Codetoextract.ipynb`) > CalenderPDF
- Reads the exported **BlueCourses.csv** file from the O drive:
- Filters rows by semester (e.g. `"Spring/Summer 2025"`)
- Groups by **Part Of Term**
- Aggregates:
- Course Start / End Dates  
- SOQ (Evaluation) Start / End Dates  
- Outputs a clean file: NEWSOQCalender.xlsx
- Enter the dates to the word file "2025_fallDatesSOQs" note some of th POT survey start and end have the same dates which you will have to adjust that based on course start and end date (see screenshot)
- Convert to PDF and upload to Googledrive
- Update SOQ calender in Canvas faculty and dean hub and Fillout and SM email templates 

---
POT that have the same survey start and end date need to be changed to the course start and end dates

<img width="864" height="538" alt="image" src="https://github.com/user-attachments/assets/901c1e93-b5aa-432a-bb32-92e1b073fdd0" />

---

