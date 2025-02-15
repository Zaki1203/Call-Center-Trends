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
Dataset used for this task was presented by [PWC](https://www.pwc.ch/en/careers-with-pwc/students/virtual-case-experience.html) and call centre trends dataset:

## Tools

I utilized Excel for data cleaning and Power BI for developing the dashboard.

Dataset: [Call Centre Trends](https://github.com/Zaki1203/Call-Center-Trends)

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

Answered = CALCULATE(COUNT(Sheet1[Call Id]),FILTER(Sheet1,Sheet1[Answered (Y/N)]="Y"))
Not Answered = CALCULATE(COUNT(Sheet1[Call Id]),FILTER(Sheet1,Sheet1[Answered (Y/N)]="N"))
Resolved Call = CALCULATE(COUNT(Sheet1[Call Id]),FILTER(Sheet1,Sheet1[Resolved]="Y"))

## Data Visualization (Dashboard) 

Dashboard

Shows visualizations from Call Center Trends :

<img width="607" alt="image" src="https://github.com/user-attachments/assets/50eaebd0-540a-4556-aed9-03433644879d" />
