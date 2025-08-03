# 🇫🇷 French Population Statistics (1968–2020)

This project analyzes demographic trends in France from 1968 to 2020 using census data. The goal was to create a normalized relational database and generate meaningful statistical and visual insights on population growth, density, and regional dynamics.

## 👨‍💻 Authors
- William Smith  
- Romain Jaffuel  
- Florian Grolleau  
- Léandre Testart

## 📅 Academic Project
- **University:** CY Université  
- **Instructor:** Renaud Verin  
- **Date:** December 16, 2024

---

## 📊 Project Objective

The objective was to transform raw census CSV files into a structured SQL database and use Python (Pandas + Matplotlib) to extract and visualize key statistics. We focused on:
- Changes in population across cities, departments, and regions
- Birth and death rates
- Evolution over time

---

## 🗂️ Data Sources

The project uses CSV data files containing:
- City-level population information
- Department and region identifiers
- Annual birth and death statistics

---

## 🏗️ Methodology

### 📐 Database Design
We created both a Conceptual Data Model (MCD) and Logical Data Model (MLD) featuring entities such as:
- `Commune` (City)
- `Departement` (Department)
- `Region`
- `Population`, `Birth`, and `Death`
- A relation `Enregistrer` to link population, births, deaths, and years

### 🛠️ Data Processing
- Cleaned and standardized CSVs using Python:
  - Managed delimiters (`;`, `,`)
  - Renamed columns for MySQL compatibility
  - Ensured structural integrity of files
- Loaded data into MySQL using SQLAlchemy and pandas
- Stored corrected versions for reproducibility

---

## 🧪 Results

### ✅ Key Queries and Visualizations
- Top 10 cities with highest population growth (1968–2020)
- Population evolution by region and department
- Birth/death comparisons by year and location
- Handling of special DROM-COM codes
- Growth rates in percent by region

Visualizations were created using Matplotlib and saved as image files.

---

## ⚠️ Challenges

- Inconsistent CSV formatting and headers
- Difficulty connecting Spyder to MySQL (switched to VS Code)
- Merging multiple datasets into consistent relational tables
- Handling edge cases such as overseas departments (DROM-COM)

---

## 📌 Conclusion

This project provided a practical and technical experience in handling real-world population data. We applied SQL and Python to build a reliable and queryable database. Despite various challenges, we were able to extract meaningful insights and visualizations.

---

## 🧰 Technologies Used

- Python (pandas, SQLAlchemy, matplotlib)
- MySQL
- Visual Studio Code

---
