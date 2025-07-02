# 📊 Data Science Salary Calculator

An interactive salary dashboard built in Microsoft Excel that allows users to explore compensation trends across various Data Science roles worldwide.  
No Power BI required — designed entirely using Excel's built-in capabilities.

---

## 🎯 Project Objective

The goal of this project was to create a user-friendly salary calculator that estimates median salary ranges based on:

- 🧑‍💻 **Job Title**
- 🌍 **Country**
- 🏢 **Work Type** (Remote, Hybrid, On-site)

The tool delivers filtered insights using dynamic calculations and responsive charts — empowering users to evaluate job market trends quickly and intuitively.

---

## 📁 Dataset

- Source: *Excel for Data Analytics* course by Luke Barousse and Kelly Adams
- Year: 2023  
- Content: Real-world data covering job titles, locations, salary ranges, and required skills across the Data Science field

---

## 🧠 Key Features

- 📈 **Bar & Column Charts** – Display median salary levels across job roles  
- 🗺️ **Map Chart** – Highlights geographic salary differences using a color scale  
- 🔢 **Median Salary Calculator** – Advanced formula with multi-criteria filtering (Job Title, Country, Schedule Type)  
- 📋 **Unique Job Types Counter** – `FILTER()`-based formula to derive clean, validated job type lists  
- ✅ **Data Validation Lists** – Ensure consistent input for dropdown filters (e.g., Job Title, Country)

---

## 🧰 Excel Features & Skills Used

| Category              | Tools & Techniques                                                                 |
|-----------------------|-------------------------------------------------------------------------------------|
| Data Preparation      | Cleaned & validated data directly within Excel                                      |
| Formulas & Functions  | `MEDIAN()`, `IF()`, `FILTER()`, `UNIQUE()`, array logic                            |
| Visualization         | Bar Charts, Column Charts, Map Chart, Conditional Formatting                       |
| Interactivity         | Dropdown selectors via Data Validation                                              |
| UX Design             | Clear layout, color-coded visuals, intuitive structure                             |

---

## 📸 Dashboard Preview

![PageView](https://github.com/bartoszsmielowski/Excel_DataScienceSalaryCalculator/blob/main/003%20Multimedia/DataScienceSalaryCalculator_PageView.png)

---

## 🧪 Example Formulas

**Median Salary by Role:**
```excel
=MEDIAN(IF((Job=selectedJob)*(Country=selectedCountry)*(Type=selectedType)*(Salary<>""), Salary))
