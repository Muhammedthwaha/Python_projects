
# 📊 Employee Survey Data Analysis

*A Data Cleaning, Transformation, and Insight Generation Project using Python (Pandas)*

---

## 📁 **Project Overview**

This project focuses on analyzing employee survey data exported from SurveyMonkey.
The raw dataset contained multiple issues such as:

* Duplicate columns
* Missing values
* Mixed question formats
* Long text-based survey questions
* Unstructured response formats

To solve this, a Python-based data cleaning and transformation pipeline was created.
The final output is a clean, analysis-ready dataset suitable for Power BI, Tableau, or further statistical analysis.

---

## 🔧 **Key Tasks Performed**

### ✔ 1. **Data Cleaning & Preprocessing**

* Removed unnecessary columns
* Cleaned messy survey question strings
* Handled missing values using conditional filtering
* Standardized employee attributes:

  * Division
  * Position
  * Generation
  * Gender
  * Tenure
  * Employment Type

### ✔ 2. **Data Transformation**

* Reshaped survey responses into a row-wise format
* Extracted question names
* Counted how many respondents selected each answer
* Added a `same_answer` count column
* Created a final consolidated dataset ready for visualization

### ✔ 3. **Dataset Outputs**

Your project generates the following files:

| File                                        | Description                                                           |
| ------------------------------------------- | --------------------------------------------------------------------- |
| **Data - Survey Monkey Output Edited.xlsx** | Cleaned employee demographic data                                     |
| **Final_output.xlsx**                       | Fully transformed dataset with answers, counts, and structured labels |
| **Script1 - Data_Manipulation.ipynb**       | Jupyter notebook containing all cleaning and transformation code      |
|**Data - Survey Monkey Output .xlsx**        | Initial Data (Raw Data)

---

## 📂 **Project Structure**

```
📁 Employee-Survey-Analysis
│
├── Data - Survey Monkey Output Edited.xlsx
├── Final_output.xlsx
├── Script1 - Data_Manipulation.ipynb
│
└── README.md
```

---

## 📌 **Technologies Used**

* **Python**

  * Pandas
  * NumPy
* **Jupyter Notebook**
* **Excel (for initial review)**

---

## 📈 **Key Insights (from the sample of data previewed)**

* Infrastructure and Finance divisions have the highest participation.
* Most respondents are **Full-time Employees** across all divisions.
* A significant portion of respondents belong to **Generation X** and **Millennials**.
* Tenure ranges vary widely, with many employees having **10+ years** of experience.
* The `same_answer` metric helps identify which answers were most common for each question.

(*If you want, I can generate more insights after reviewing the full dataset.*)

---

## 🚀 **How to Use This Project**

1. Open **Script1 - Data_Manipulation.ipynb**
2. Run the notebook step-by-step
3. The script will:

   * Load raw data
   * Clean & structure it
   * Export: **Final_output.xlsx**
4. Use the final file in:

   * Power BI
   * Tableau
   * Excel dashboards
   * Statistical models

---

## 📬 **Contact**

**Muhammed Thaha Uwais**
📧 *[muhammedthahauwais@gmail.com](mailto:muhammedthahauwais@gmail.com)*
🔗 *LinkedIn:* [https://www.linkedin.com/in/muhammed-thaha-uwais-5b5444279/](https://www.linkedin.com/in/muhammed-thaha-uwais-5b5444279/)

---

