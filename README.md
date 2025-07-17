
# Hospital Emergency Room Analysis Dashboard

**Live Dashboard:** [Access the Power BI Report](https://app.powerbi.com/groups/me/reports/a1d8d255-3488-4a89-8811-4b308a41f3f0/0b9fbc8c6dbc6ba0c3bc?experience=power-bi)

---

## Overview

This Power BI dashboard offers a detailed examination of Emergency Room (ER) operations within a hospital setting. By consolidating patient flow, wait times, referral sources, and admission rates into an integrated interface, the report enables stakeholders to monitor performance, identify trends, and support strategic decision-making.

## Purpose

Emergency departments often contend with overcrowding, extended wait periods, and variable admission rates, all of which can affect patient outcomes and satisfaction. This dashboard was developed to address the following objectives:

- Monitor monthly and longitudinal trends in ER metrics.
- Identify peak demand intervals by hour and day.
- Assess the relationship between wait times and patient satisfaction.
- Determine referral volumes by department.
- Facilitate in-depth review of individual patient encounters.

---

## Data Description

- **Source File:** `Hospital ER_Data.csv` (April 2023 to October 2024)
- **Fields Included:**
  - Check-in and check-out timestamps
  - Patient demographics (age group, gender, race)
  - Department referral and admission status
  - Calculated wait times and satisfaction scores

---

## Methodology

1. **Data Preparation**

   - Imported the CSV file into Power BI Desktop.
   - Standardized date/time formats and addressed missing values.
   - Derived additional columns for Month, Year, and Hour segments.

2. **Data Modeling**

   - Established a Date dimension table to enable time-series analysis.
   - Defined relationships between lookup tables (e.g., departments).
   - Created DAX measures for key indicators: total visits, average wait time, satisfaction rate, referral counts, and service-level compliance (≤30 minutes).

3. **Report Design**

   - **Monthly Analysis:** KPI cards, bar and donut charts to present summary metrics.
   - **Trend Analysis:** Line and stacked bar charts to illustrate changes over time.
   - **Patient Detail View:** Interactive table with slicers for date range, department, and admission outcome.
   - Included interactive elements such as tooltips, drill-through capabilities, and slicers for dynamic filtering.

4. **Styling and Deployment**

   - Applied a consistent color scheme and typography for enhanced readability.
   - Annotated visuals with descriptive titles and data callouts.
   - Published the report to the Power BI Service and configured access permissions.

---

## Summary & Key Insights (April 2023 – October 2024)

### Descriptive Analysis

- **Total Unique Patients:** 9,216

### Patient Wait Time & Satisfaction

- **Average Wait Time:** 35.3 minutes, indicating potential areas for process efficiency.
- **Average Satisfaction Score:** 4.99/10, suggesting moderate satisfaction levels and a need for experience enhancement.

### Departmental Referrals

- **No Referral Required:** 5,400 patients
- **Top Referral Departments:**
  - General Practice: 1,840 cases
  - Orthopedics: 995 cases
  - Physiotherapy: 276 cases
  - Cardiology: 248 cases

### Peak Busy Periods

- **Busiest Days:**
  - Monday: 1,377 patients
  - Saturday: 1,322 patients
  - Tuesday: 1,318 patients
- **Busiest Hours:**
  - 11 AM, 7 PM, 1 PM, and 11 PM

### Patient Demographics

- **Top Age Groups:**

  - 30–39 years: 1,200 patients
  - 20–29 years: 1,188 patients
  - Also notable: 40–50 years

- **Race Distribution:**

  - White: 2,571
  - African American: 1,951
  - Multiracial: 1,557
  - Asian: 1,060
  - Declined to identify: 1,030

### Admission Patterns

- **Admitted Patients:** 4,612
- **Treated & Released:** 4,604

### Final Summary

The dashboard uncovers high ER utilization, with a fairly even split between admitted and non-admitted cases. Peak activity is observed on Mondays and during late evenings, suggesting a need for targeted resource deployment. Referral patterns emphasize demand in General Practice and Orthopedics, while patient satisfaction levels call for improvements in service delivery. The demographic analysis reveals a diverse patient base, underscoring the importance of inclusive and responsive care strategies.

---

## Repository Structure

```
Hospital ER_Data.csv  # Raw patient visit dataset
powerBI hospital data project .pdf # Pdf file of Project
powerBI hospital data project.pbix # Power BI project file
README.md                 # This documentation file
```

---
