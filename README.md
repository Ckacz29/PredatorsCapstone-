# PredatorsCapstone

Create a workflow that draws data from the Google Analytics platform.

---

##  Project Overview

I am helping the **Nashville Predators' Business Strategy** team gather insights into their [NHL.com/predators](https://NHL.com/predators) webpage. The current process of collecting Google Analytics data is **manual, inefficient, and prone to data loss**.

By implementing an **automated KNIME workflow** that extracts, transforms, and stores Google Analytics data in **CSV format** for easy Tableau integration, we can enable **data-driven decision-making** across departments. This not only **saves time** but also ensures that data is **clean and easily distributed** to stakeholders.

---

##  Problem Statement

The Nashville Predators' analytics team has **not prioritized Google Analytics** due to the manual effort required to filter data through the platform. The team currently uses it only for quick reference because:

- **Data extraction is time-consuming**
- **Formatting is inconsistent**
- **Insights are delayed**

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

## ⚙️ Technical Stack

- **KNIME** – for ETL workflow
- **Google Drive ** – for cloud-based CSV storage
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


---

##  Key Learnings

- Gained mastery in **KNIME** for enterprise-level ETL
- Practiced professional communication with real-world stakeholders and teams

---

##  Repository Links 
- KNIME workflow .knwf (attatched at top)
- Tableau Workbooks:
     - https://public.tableau.com/views/PredsTicketConversions/TicketConversions?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
     - 



---










Sprint retorspectives: 

#Sprint 1
In the first sprint, the goal was to extract and clean data the Nashville Predators google analytics service. I was able to complete this through KNIME with a series of node loops that looped my query's from October to March. 


#Sprint 2
There were multiple goals in this sprint. First of which was extracting data from my previous for loop to gather insight on the Nashville Predators article performance and ticket landing pages. The next step was to put this article data into a tableau dashboard to show the top performing articles from the year. The last goal, which was not accomplished, was to automate Tableau through it's S3 server connector. I created an S3 bucket to store my csv. KNIME has an s3 node that makes it easy to upload files there. From there I was able to get Tableau to recognize my file, however the data would come up blank. Looking at forums some people have had similar issues with no resolve. I tried to create an Athena table to pointed to the bucket and connect it that way with no success either. 

#Sprint 3
The goal of this sprint was to create a tabluea dashboard that gave insight into to the conversion rate vs. revenue for single game tickets and how website traffic could have affected those results. Using KNIME I pulled total amount of views each game had, the total revenue, and amount of tickets purchased. From there I was able to create a scatter plot that showed the relation between conversion rate and item revenue. Using KNIME again, I pulled page path data that allowed me to see the total amount of webtraffic before a game, but also what specific pages were being visited leading up to the game. The biggest challenge throughout this sprint was cleaning the data. Google Analytics returned the same game twice with different dates. I had to manipulate the strings that had the wrong date so that they would match the correct date and then concatenate the two records so they had the correct data. 












