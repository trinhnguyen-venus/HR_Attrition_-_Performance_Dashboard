# 📊 HR Performance Dashboard

## Skills Demonstrated
Power Query: 	Data extraction, transformation, and automation
Power Pivot (DAX):	Measure creation, KPI computation, and relationships
Pivot Table / Pivot Chart:	Multi-dimensional HR analysis
Dashboard Design:	Layout, formatting, and storytelling with visuals

---

## Project Overview
This project demonstrates advanced Excel analytics skills through the creation of a fully interactive **HR Analytics Dashboard**.  
It highlights the end-to-end analytical process — from data cleaning, modeling, and KPI calculation to dashboard design — using Excel’s modern tools:
- **Power Query** for ETL (Extract – Transform – Load)
- **Power Pivot** for Data Modeling and DAX calculations
- **Pivot Table & Pivot Chart** for analysis
- **Dashboard Design** for professional visualization and insights delivery

---

## ⚙️ Project Workflow

### Step 1 — Import Data (Power Query)
- Source: `HR_raw_data.xlsx`  
- Actions: import into Power Query, detect and fix column types, remove unneeded columns, handle missing values, normalize formats.
- Result: a cleaned data query ready to load into an Excel Table.

![Step 1 - Import Data](images/Step1_Import_Data.png)


### Step 2 — Data Cleaning & Transformation
- Actions:
  - Standardize date/number/text formats.
  - Create derived columns (e.g. `AgeBand`, `WorkYears`).
  - Remove duplicates and validate key columns.
- Result: clean dataset and a Data Validation table verifying integrity.

![Step 2 - Cleaning Data](images/Step2_Cleaning_Data.png)
![Data Validation Table](images/Data_Validation_Table.png)


### Step 3 — Load to Excel Table (`HRData`)
- Load cleaned query into an Excel Table named **HRData**.  
- Create `KPI_Table` documenting KPI definitions, calculation formulas, and targets.
- This table acts as the single source of truth for downstream analysis.

![Step 3 - Load HRData](images/Step3_Load_HRData.png)
![KPI Table](images/KPI_Table.png)


### Step 4 — Data Model & Measures (Power Pivot / DAX)
- Add `HRData` into the Data Model (Power Pivot).  
- Implemented DAX measures for KPIs:

  ```DAX
  Headcount = DISTINCTCOUNT([EmployeeNumber])
  TurnoverCount = CALCULATE( COUNTROWS(HRData), HRData[Attrition] = "Yes")
  TurnoverRate = DIVIDE( [TurnoverCount], [Headcount], 0 )
  PercentOverTime = AVERAGE(HRData[OverTime])
  AvgMonthlyIncome = AVERAGE(HRData[MonthlyIncome])
  AvgJobSatisfaction = AVERAGE(HRData[JobSatisfaction])
```

###Step 5 — Pivot Tables & Visuals

Built PivotTables by key HR dimensions:

Department: Headcount, Turnover Rate, Promotion Rate, Avg Income

Gender: Turnover Rate by Gender

Job Role: Avg Monthly Income by Job Role


### Step 6 — Dashboard Design

Combined visuals into an interactive HR Dashboard.

Applied consistent color palette, gradient columns, and slicers for filters.

Key visuals include:

Avg Monthly Income by Job Role

Turnover Rate by Department

Gender Diversity Overview

![Dashboard](images/Dashboard.png)

---

## 💡 Key Insights (summary)

Turnover hotspots: Sales roles show the highest turnover; investigate workload and compensation alignment.

Compensation: Managers and research directors have the highest average incomes; review pay bands for lower-paid roles.

Workload & Satisfaction: Higher overtime correlates with lower job satisfaction — consider workload redistribution or wellbeing programs.

Experience impact: Employees with longer tenure generally have higher performance ratings.


## Author
**Trinh Nguyen**  
📧 Contact: ng.trinh3023@gmail.com
📍 GitHub: [https://trinhnguyen-venus.github.io/](https://trinhnguyen-venus.github.io/)
