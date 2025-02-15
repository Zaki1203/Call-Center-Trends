# Call-Center-Trends

##  Project Overview
I developed a Call Center Trends Analysis Dashboard using Power BI to monitor and analyze the performance of call center agents from January 1, 2021, to March 31, 2021. 

## Objectives 
The objective of this project is to design and develop a Power BI dashboard for the call center manager, providing a comprehensive view of key performance indicators (KPIs) and essential metrics derived from the dataset. The dashboard will enable data-driven decision-making by presenting insights such as:  

- Overall customer satisfaction  
- Total calls answered vs. abandoned  
- Call volume distribution over time  
- Average speed of answer (ASA)  
- Agent performance quadrant, analyzing average handle time (talk duration) against calls answered  

The goal is to deliver an intuitive, interactive dashboard that supports performance monitoring, operational efficiency, and strategic improvements within the call center.

## Data Source
Dataset used for this task was presented by [PWC](https://www.pwc.ch/en/careers-with-pwc/students/virtual-case-experience.html) and call centre trends Dataset: [Call Centre Trends](https://github.com/Zaki1203/Call-Center-Trends)

## Tools

I utilized Excel for data cleaning and Power BI for developing the dashboard.



## Process
Open Microsoft Power BI, navigate to **Get Data**, and select **Excel**. Locate and open the file named **"01 call-center-dataset"**. Once the data is loaded, click on **Transform Data** to access Power Query and perform basic data transformations.  

Upon inspecting the dataset, I observed that it contains 10 columns with the following names:  
- Call Id
- Agent
- Date  
- Time
- Topic
- Answered
- Resolved
- Speed of Answer (in seconds)
- Avg Talk Duration
- Satisfaction Rating

I reviewed the data types of all columns to ensure accuracy and consistency. Additionally, I performed basic data cleaning by removing unnecessary rows to improve data quality and reliability.

## Dax 
Measures used in all visualization are:

-Answered = CALCULATE(COUNT(Sheet1[Call Id]),FILTER(Sheet1,Sheet1[Answered (Y/N)]="Y"))

-Not Answered = CALCULATE(COUNT(Sheet1[Call Id]),FILTER(Sheet1,Sheet1[Answered (Y/N)]="N"))

-Resolved Call = CALCULATE(COUNT(Sheet1[Call Id]),FILTER(Sheet1,Sheet1[Resolved]="Y"))

## Data Visualization (Dashboard) 

Dashboard

Shows visualizations used in Call Center Trends :

-Pie chart- Shows the count of answered and resolved calls 

-Stacked Column chart-shows number of calls per month

-Guage-shows the average satisfacory rating 

-Matrix-Presents the statistics for each agent.

-card-Displays the average speed of answer in seconds.

<img width="607" alt="image" src="https://github.com/user-attachments/assets/50eaebd0-540a-4556-aed9-03433644879d" />

# Slicers
-Date Slicer- Allows user to change the date according 

-Topic Slicer-Allowes user to select the topics

-Agent slicer -allows user to select the agent 

## Key Insights

-Most calls are answered in the month of the jan 1455

-Most of the satisfaction ratings from each call are 3 and 4.

-The average speed of answer by Joe is the highest.

-The call resolution rate of Jim is the highest, even though the average speed of his answers is lower compared to those of Joe, Martha and Dan. The call answered by - him are also higher than the average number of calls answered.

-Becky's speed of answer is the lowest among all, and her rate of calls resolved is higher. She is in the 5th position in the call resolution rate.

-Martha has the highest speed of answered in the sec

-Diana has highest count of not answering the call

-Most of the calls received are for admin support 


