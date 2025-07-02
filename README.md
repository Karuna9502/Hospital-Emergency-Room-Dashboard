# Hospital-Emergency-Room-Dashboard -Excel Project
This is an interactive dashboard built entirely in Excel to analyze and visualize Emergency Room (ER) data. It helps monitor key hospital performance metrics like patient wait time, department referrals, and patient demographics.

🔄 Step-by-Step Workflow
1️⃣ Business Requirement Gathering
Identified the need to track:

Admission Status

Patient Demographics (Age, Gender)

Timeliness of care

Department Referrals

Overall patient satisfaction

2️⃣ Understanding of Data
Analyzed the raw hospital ER dataset to understand:

Data columns and types

Patterns and key measures

Relationships between patient, time, and departments

3️⃣ Data Connection
Imported and prepared the data in Excel sheets using manual inputs and formulas.

4️⃣ Data Cleaning & Quality Check
Removed duplicates and corrected formatting issues.

Ensured accuracy in age groups, genders, dates, and referral categories.

5️⃣ Creating Calendar Table (Using Formulas)
Created a month-wise slicer and year filter for dynamic report filtering.

6️⃣ Data Modeling (Manually in Excel)
Structured the data using separate sheets for:

Raw Data

Cleaned Data

Pivot Tables

Dashboard

7️⃣ Calculations (Using Dax Formulas)
DAX Formula for Age Group : 
=IF([Patient Age]>=70,"70-79",IF([Patient Age]>=60,"60-69",IF([Patient Age]>=45,"45-59",IF([Patient Age]>=30,"30-44",
IF([Patient Age]>=15,"15-29",IF([Patient Age]>=5,"05-14","0-4"))))))

DAX Formula For Patient Attend Status :
=IF([Patient Waittime]<30,"Within Time","Delay")

= List.Dates(#date(2023,01,01),731,#duration(1,0,0,0))


8️⃣ Pivot Tables & Dashboard Layout
Created pivot tables to summarize data for:

Gender distribution

Timeliness

Age groups

Referral departments

Linked the pivot tables to slicers (Month, Year)

9️⃣ Chart Development & Formatting
Designed visuals using:

Pie Charts (Gender, Timeliness)

Bar Charts (Age Group, Referrals)

Cards for KPIs (No. of Patients, Avg. Wait Time, Satisfaction Score)

Applied consistent color themes and icons for clarity.

🔟 Dashboard Design & Interactivity
Assembled all visuals into a single dashboard sheet.

Added slicers for months and years to make it interactive.

1️⃣1️⃣ Insight Generation
Found that:

52% patients were non-admitted.
30–39 age group had the highest ER visits.
General Practice received the most referrals.
Average wait time was around 34.43 mins
Patient satisfaction was 5.16

🛠 Tools Used

Microsoft Excel
Pivot Tables
Slicers
Charts & Visual Formatting

📷 Dashboard Preview
(Add dashboard screenshot image here when uploading to GitHub)

📁 Repository Includes:
Excel File (.xlsx)

Screenshot of Final Dashboard

ReadMe Documentation
