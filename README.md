# -Hr-Dashboard-Excel---SSIS---SQl-server-dbs---POWER-BI
The Applicants Dashboard was built to help the company management and recruitment team analyze applicant data from the 2026 season.
##  Project Overview

The challenge began when the recruitment form responses were collected through a Google Sheet, which was messy, inconsistent, and lacked data standardization.  
As a data engineer and analyst, I designed a complete ETL (Extract–Transform–Load) workflow and developed an interactive Power BI dashboard to answer key questions about applicants’ demographics, interests, and engagement.



---
![Screenshot 2025-10-12 152012](https://github.com/user-attachments/assets/73d34e06-bf9e-4112-8e03-746a5ca126f1)


![Screenshot 2025-10-12 152029](https://github.com/user-attachments/assets/2d5fd743-ba3c-4d34-bc76-dcee640ed7ad)




##  Workflow Summary

### 1️ Data Extraction
- Exported raw dataset from Google Sheets as an Excel file.  
- The data contained non-standardized text fields, inconsistent formats (like “AAST” vs “Arab Academy”), and missing values.

### 2️ Data Transformation (Power Query)
- Cleaned and transformed data using Power Query in Power BI.  
- Standardized values across all categorical columns:
  - Unified university names, faculties, and departments.  
  - Converted text-based graduation years to integers.  
  - Extracted and formatted date and time from timestamps.  
  - Handled missing and duplicate entries.  
  - Renamed columns for clarity and consistency.
 
  - <img width="737" height="1295" alt="image" src="https://github.com/user-attachments/assets/98a5a30b-3673-4be3-afda-fbb2c6125d6b" />


### 3️ Data Loading (SSIS + SQL Server)
- Automated the loading pipeline using SQL Server Integration Services (SSIS).  
- Configured an SSIS data flow to load the cleaned Excel file into SQL Server.  
- Created the target table schema in SQL Server:

  ```sql

 

-<img width="795" height="1200" alt="Screenshot 2025-10-15 140301" src="https://github.com/user-attachments/assets/bb1646a9-eb2c-4daa-b45e-03aa962abba8" />


  
## 📊 Power BI Dashboard Design

### Page 1 – Overview
High-level summary for executives and recruitment team.

**KPIs (Cards):**  
- Total Applicants  
- Male vs Female Ratio  
- Most Common University  
- Most Common Field to Join  
- Highest Term Applying  

**Visuals:**  
- Line chart → Applications over time (from 4/9 to 12/9)  
- Bar chart → Applicants by University  
- Treemap → Distribution by Field to Join  
- Pie chart → Gender distribution  
- Column chart → Applicants by Graduation Year  

**Purpose:**  
Gives a snapshot of application activity, top institutions, and participation trends.

---

### Page 2 – Detailed Insights
Focused on understanding motivation, experience, and engagement.

**KPIs (Cards):**  
- % of applicants with previous competition experience  
- % of applicants who asked questions  
- % of applicants from Computer-related faculties  

**Visuals:**  
- Stacked bar chart → Working Hours Preferences by Gender  
- Word cloud / table → Why Join the Club (common motivations)  
- Horizontal bar chart → Previous Competitions participated in  
- Pie chart → Platform used to apply (LinkedIn, Instagram, etc.)  
- Matrix/Table → Cross-analysis of Term vs Field to Join  

**Purpose:**  
Helps recruitment leads identify the most engaged applicants, popular motivation factors, and potential training focus areas.

---

  ## ☁️ Technologies Used

| Tool                         | Purpose                                      |
|-------------------------------|---------------------------------------------|
| Power Query (Power BI)        | Data cleaning and transformation            |
| SSIS (SQL Server Integration Services) | ETL and loading data into SQL Server |
| SQL Server                    | Centralized data storage                     |
| Power BI                      | Data visualization and analytics            |
| Excel / Google Sheets         | Original data source                         |

---

##  Business Impact
- Turned messy, inconsistent Google Sheet data into clean, reliable structured data.  
- Delivered a real-time, interactive dashboard to decision-makers.  
- Simplified tracking of applicant demographics, engagement, and growth trends.  
- Enabled data-driven recruitment decisions for the 2026 season.

note: fabricated the data  before uploading for security and didn't add any files for privacy

