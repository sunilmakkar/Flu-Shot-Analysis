# Flu Shots Dashboard - Data Analytics Case Study

## 1. Objective

The goal of this project was to analyze and visualize a healthcare system’s **2022 flu shot compliance** using patient demographics and immunization records. Specifically, we sought to identify:

- **Flu shot uptake** by age, race, and county.
- **Overall compliance** percentage (i.e., % of the active patient population who received a flu shot).
- **A running total** of flu shots administered throughout 2022.
- A **patient list** highlighting who did or did not receive a flu shot.

By synthesizing this information, healthcare administrators can more effectively allocate resources and target populations with the **lowest compliance rates**.

## 2. Executive Summary

In this analysis, we combined patient demographic data with immunization records (focusing on seasonal flu shots in 2022). After cleaning and transforming the data in SQL, we visualized it in Tableau to produce a **dashboard** that shows:

- Total Flu Shots Given: 4,023
- Total Compliance: ~81.7%
- Age Group Breakdowns: Flu shot compliance ranges from ~64.8% for 18-34 age group to ~95.6% for 50-64.
- Racial Disparities: Compliance ranges from ~75% in “Other” to ~93.8% in “Native” populations.
- Geographical Spread: Counties show varying rates, which can be mapped for targeted intervention.
- Running Monthly Totals: A clear month-by-month cumulative increase in administered flu shots.

### Key Outcomes for Decision-Makers

1. **High overall compliance** near 82%—but there is room for improvement in certain age ranges and racial groups.
2. **Targeted outreach** opportunities exist for the 18-34 group (64.8% compliance) and “Other” race category (75%).
3. **The cumulative running total** demonstrates steady growth, indicating that consistent promotional efforts throughout 2022 were effective.

## 3. Tools Used

1. SQL – Data extraction and cleaning (joins, CTEs, and filtering for 2022 flu shots).
2. Tableau – Data visualization and interactive dashboard design.
3. Spreadsheet/CSV – Optional step for those who prefer not to connect directly to a database.

## 4. Project Sections

### 4.1 Data Preparation (SQL)

- Data Sources: Patients, Immunizations, and Encounters tables.
- Filtering: Restricted records to active patients with encounters after 2020, alive (no death date), and at least six months old by end of 2022.
- Aggregation: Used group statements to identify earliest flu shot date in 2022 per patient.
- One-to-One Relationship: Ensured immunization records matched to unique patients by restricting duplicates.
- Flu Shot Indicator: Created a binary (flu_shot_2022 = 1 if given, 0 if not).

### 4.2 Dashboard Construction (Tableau)

1. **Compliance by Age**
- Bar chart illustrating flu shot compliance across 0-17, 18-34, 35-49, 50-64, and 65+ age groups.

2. **Compliance by Race**
- Bar chart comparing flu shot percentages for major racial categories.

3. **Flu Shot % by County**
- A filled map to identify geographic patterns and highlight counties with lower vaccination rates.

4. **Flu Shots List**
- A table listing patient names and whether they received a flu shot. Useful for follow-up outreach.

5. **Running Sum of Flu Shots (2022)**
A cumulative graph illustrating how many patients received the vaccine month by month.

## 5. Business Insights & Visualizations

### *Insight 1: Under-35 Age Group Lags*
- **Finding:** Only ~64.8% of patients aged 18–34 received the flu shot, significantly below the overall 81.7%.
- **Business Action:** Focus marketing campaigns on younger adults (e.g., workplace flu clinics, social media awareness).

### *Insight 2: Racial Disparities in Compliance*
- **Finding:** The “Native” group exhibited the highest compliance (93.8%), while the “Other” category trailed at ~75%.
- **Business Action:** Investigate the reasons behind these disparities—possibly language barriers or access issues—and tailor community engagement to boost coverage in lower-performing groups.

### *Insight 3: Geographical Variation*
- **Finding:** Certain counties consistently show lower uptake, while others surpass the 80% average.
- **Business Action:** Health system planners can allocate additional mobile clinics or resources to underperforming regions.

### *Insight 4: Steady Uptake Over Time*
- **Finding:** The cumulative running total shows a steady increase throughout the year, peaking in early fall.
- **Business Action:** Reinforce marketing efforts ahead of flu season (August–October) to encourage early vaccination.

### *Insight 5: Targeted Outreach Lists*
- **Finding:** A patient list reveals exactly who did not receive the 2022 flu shot.
- **Business Action:** Leverage call centers or automated messaging to reach out directly, offering convenient scheduling or reminders.

## Conclusion

**Overall**, this project shows how integrating **SQL** data extracts with an intuitive **Tableau** dashboard can arm healthcare providers with **actionable insights**. By focusing on **demographic segments** and **geographic hotspots** where compliance is low, organizations can **optimize resources** and **improve patient outcomes**.

### **Next Steps:**
- **Extend the analysis to track influenza hospitalizations vs. vaccination status.**
- **Add other immunizations (e.g., COVID-19 boosters) to get a more comprehensive picture of population health.**

## How to Aceess the Project

**1. SQL Scripts & Data**: 
**2. Tableau Workshop**: 
**3. Project Documentation**: 
