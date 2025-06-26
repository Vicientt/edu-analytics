# UCI EDU ANALYTICS – Student Learning Behavior Project

## 📘 Project Overview

This project analyzes student learning behavior using the Open University Learning Analytics Dataset. It is divided into three main stages across three working days. The analysis is conducted in Databricks using SQL only.

---

## 📅 Project Workflow

### Day 1: Data Setup & Git Integration

- Set up Databricks workspace and connect GitHub repo.
- Upload raw dataset files: `studentInfo.csv`, `studentRegistration.csv`, `studentAssessment.csv`, `studentVle.csv`.
- Create initial SQL tables from the CSV files.
- Push notebooks and files to the GitHub repository.

### Day 2: Data Cleaning & Merging

- Perform EDA (Exploratory Data Analysis) on individual tables.
- Clean invalid/missing data (e.g., dates with question marks).
- Create the following cleaned or merged views:
  - `v_student_info`: Cleaned version of `studentInfo`.
  - `v_student_registration_cleaned`: With properly formatted and filtered registration dates.
  - `v_student_vle`: Cleaned VLE interactions.
  - `v_student_assessment_cleaned`: Filtered scores with valid integers.
- Then, create final merged views for deeper analysis:
  - `v_student_summary`: General student-level info.
  - `v_vle_summary`: Aggregated click counts.
  - `v_assessment_score`: Assessment metrics by student.
  - `v_student_timeline`: Derived registration periods (duration of participation).

### Day 3: Result Analysis & Dashboard

Use final views to perform descriptive SQL analysis and visualize results.

- **final_result_distribution**: Distribution of student outcomes (Pass, Fail, Withdrawn, Distinction).
- **clicks_vs_score**: Compare average clicks and average scores grouped by final result.
- **ageband_summary**: Clicks and outcomes grouped by age band.
- **registration_days_summary**: Summary of learning days by final result.
- **course_analysis_summary**: Number of students, assessments submitted, and performance by course.
- **engagement_summary**: Engagement metrics including average clicks and duration across courses.

---

## 📁 Folder Structure

```
UCI_EDU_ANALYTICS/
│
├── dataset/                     # Raw CSV files
├── 01-create-table.ipynb       # Create tables from CSV files
├── 02 - EDA.ipynb              # Data cleaning and inspection
├── 03 - Merge data.ipynb       # Final view creation
├── 04 - Analyze.ipynb          # Result analysis queries
└── README.md                   # Project overview and instructions
```

---

## 🔧 Technologies Used

- Databricks Community Edition
- SQL
- GitHub for version control

---

## 👤 Author

This project was completed as an individual exercise to explore and understand student learning patterns using SQL and Databricks.
