# PredatorsCapstone

Create a workflow that draws data from the Google Analytics platform.

---

##  Project Overview

I am helping the **Nashville Predators' Business Strategy** team streamline their web analytics platform([NHL.com/predators](https://NHL.com/predators) , by developing a data pipelines that delivers faster and clearner insights, elimating the manual steps it took to utilize this data.


---

##  Problem Statement

The Nashville Predators' analytics team has **not prioritized Google Analytics** due to the manual effort required to filter data through the platform. The team currently uses it only for quick reference because:
- **Data extraction is time-consuming**
- **Formatting is inconsistent**

This limits the strategic use of web analytics for improving fan engagement and ticket revenue.

---

##  ISBA Subfields

1. **Data Engineering**  
   Use of KNIME to perform ETL (Extract, Transform, Load) from Google Analytics into CSV format for distribution aligns with core data engineering tasks.

2. **Business Intelligence & Data Visualization**  
   Integration with Tableau allows the team to build dashboards, monitor KPIs, and generate actionable insights.

3. **Digital Marketing Analytics**  
   Analyzing user behavior, engagement, and conversions from the website to improve marketing strategies and fan interaction.

---

## Solution Overview 

Drawing data from google analytics, KNIME is able to able to take this data and transform it into a csv that is both clean and usable for other application practices. The data is stored in Google Drive for easy accesability and connection to Tableau which is used to make various dashboards for insights. 

- **KNIME** – for ETL workflow
- **Google Drive** – for cloud-based CSV storage
- **Tableau** – for data visualization
- **Google Analytics 4 API**: - Data Source 


---

## 📈 Methodology: CRISP-DM Framework

| Phase                | Description                                                       |
|---------------------|-------------------------------------------------------------------|
| **Business Understanding** | Identify key traffic behaviors influencing ticket sales          |
| **Data Understanding**     | Extract GA4 event data (sessions, conversions)                |
| **Data Preparation**       | Clean and filter the data using KNIME                        |
| **Modeling**               | Create metrics like conversion rate and session value        |
| **Evaluation**             | Build Tableau dashboards with live Google Drive data feed              |


---

##  Challenges Overcome

- KNIME's learning curve for complex data manipulation
- Transition from AWS S3 to Google Drive for cloud storage
- Simplifying Dashboards for easy to read visuals 


---

##  Key Learnings

- Gained mastery in **KNIME** for enterprise-level ETL
- Keep dahsboards relatively low-level
- Practiced professional communication with real-world stakeholders and teams

---

##  Repository Links 
- KNIME workflow .knwf (attatched at top)
- Tableau Dashboards:
     - Ticket Conversions Dashboard: https://public.tableau.com/views/PredsTicketConversions/TicketConversions?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
     - Game Performance Dashboard: https://public.tableau.com/views/PredsGamePerformanceDashboard/IndividualGame?:language=enUS&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
     - Article Performace Dashboard: https://public.tableau.com/views/PredsArticlePerformance/ArticlePerformance?:language=enUS&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link


---























