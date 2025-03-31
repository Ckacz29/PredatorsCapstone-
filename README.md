# PredatorsCapstone-
Create workflow that draws data from google analytics platform 

#Project Overview
I am helping the Nashville Predators' Business Strategy team gather insights to their NashvillePredators.com webpage. The current process of collecting Google Analytics data is manual, inefficient, and prone to data loss. By implementing an automated KNIME workflow that extracts, transforms, and stores Google Analytics data in CSV format for easy Tableau integration. It will help with data-driven decision making to different departments that may rely on this information. By creating an automated workflow, 
it will save time for business strategy and the data can be easily distibuted. 

#Problem Statement
The Nashville Predators' analytics team has not prioitized the Google Analytics to track website engagement, becasue it has drawn to much effort manualy filter data through the google analytcs platform. The analytics team struggles with time-consuming data extraction and formatting. The platform is used for a quick look at the data. 

#ISBA Subfields 
1. Data Engineering - With Knime, The process of extracting data from Google Analytics, cleaning the data for easy use, and loading it into a .csv file for distrubution (ETL) correlates with main projects Data Engineers are responsible for.
2. Business Intelligence & Data Visualization – The integration of Tableau enables the Nashville Predators' analytics team to create dashboards, track KPI's, and generate insights from this data
3. Digital Marketing Analytics – This subfield focuses on analyzing user behavior, engagement, and conversions from the Nashville Predators' website using Google Analytics data to optimize marketing strategies and improve fan interactions.


Tech Stack: 
- KNIME
- Tabluea
- AWS (Athena, S3) 



#Sprint 1
In the first sprint, the goal was to extract and clean data the Nashville Predators google analytics service. I was able to complete this through KNIME with a series of node loops that looped my query's from October to March. 


#Sprint 2
There were multiple goals in this sprint. First of which was extracting data from my previous for loop to gather insight on the Nashville Predators article performance and ticket landing pages. The next step was to put this article data into a tableau dashboard to show the top performing articles from the year. The last goal, which was not accomplished, was to automate Tableau through it's S3 server connector. I created an S3 bucket to store my csv. KNIME has an s3 node that makes it easy to upload files there. From there I was able to get Tableau to recognize my file, however the data would come up blank. Looking at forums some people have had similar issues with no resolve. I tried to create an Athena table to pointed to the bucket and connect it that way with no success either. 

#Sprint 3
The goal of this sprint was to create a tabluea dashboard that gave insight into to the conversion rate vs. revenue for single game tickets and how website traffic could have affected those results. Using KNIME I pulled total amount of views each game had, the total revenue, and amount of tickets purchased. From there I was able to create a scatter plot that showed the relation between conversion rate and item revenue. Using KNIME again, I pulled page path data that allowed me to see the total amount of webtraffic before a game, but also what specific pages were being visited leading up to the game. The biggest challenge throughout this sprint was cleaning the data. Google Analytics returned the same game twice with different dates. I had to manipulate the strings that had the wrong date so that they would match the correct date and then concatenate the two records so they had the correct data. 












