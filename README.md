# Dr Abdulrahman Mahmoud's portfolio

# [Project 1: Facial recognition based attendance monitoring system](https://github.com/phdamg/phdamg.github.io)

This project is conducted for an HE institution with tens of thousands of students. The traditional method of attendance marking is a tedious task in many schools and colleges. It is also an extra burden to the faculties who should mark the attendance by manually calling the names of students which might take about 5 minutes of the entire session. Face recognition has set an important biometric feature, which can be easily acquirable and is non-intrusive. Face verification is a 1:1 matching process, it compares face images against the template face images and face identification is a 1:N problem that compares query face images. The purpose of this system is to build an attendance system that is based on face recognition techniques. Hence, the face of an individual will be considered for marking attendance.

Finalized approach
With a dataset of stored labelled faces
1.	Encode faces
2.	Detect a face using mediapipe, which detects a face in 0.01s
3.	Use the face_recognition library to identify the face, which has a 99.38% accracy.
4.	Find the person’s name from the encoding. 
5.  Store the persons name and time in a database.

![image](https://user-images.githubusercontent.com/114836975/193611560-5423d7f7-76c1-4622-896e-ffa99c526c53.png)
![image](https://user-images.githubusercontent.com/114836975/193612294-a03fbda3-7796-4389-88aa-5a3795680ef2.png)<br/><br/><br/><br/><br/><br/>



# [Project 2: Marketing Campaign Performance Monitoring for A Healthcare Company]

# Project Overview
The healthcare company runs marketing campaigns across various digital channels such as google, meta and bing to promote healthcare services such as virtual consultations, prescription delivery, and wellness packages. This project focuses on building an automated solution to monitor and analyze the performance of these campaigns. By integrating ad spend data with internal revenue data, we provide actionable insights through a Tableau dashboard tailored for non-technical stakeholders.

# Objectives
- Automate Data Integration: Combine Google Analytics (GA4) ad spend data with company revenue and patient acquisition data.
- Analyze Performance Metrics: Calculate KPIs such as:
    - Cost Per Mille (CPM)
    - Click-Through Rate (CTR)
    - Cost Per Click (CPC)
    - Conversion Rate
    - Cost Per Order (CPO)
    - Revenue Per Mille (RPM)
    - Return on Ad Spend (ROAS)
- Visualize Insights: Present the data in a Tableau dashboard with interactive features for non-technical users.

# Project Workflow
- Data Collection and Integration:
  - Extract GA4 data using Analytics Canvas.
  - Retrieve revenue and patient acquisition data from MariaDB.
  - Standardize and merge datasets into a unified format.
- Data Pipeline Design:
  - Develop an ETL pipeline to automate data extraction, transformation, and loading.
  - Create a stored procedure in MariaDB to process revenue data.
- KPI Calculation:
  - Implement field calculations in Tableau for metrics such as:
    - CTR = (Clicks / Impressions) * 100
    - ROAS = (Revenue / Ad Spend)
- Dashboard Creation:
  - Design a Tableau dashboard with:
    - Summary metrics (total ad spend, revenue, ROAS, etc.).
    - A segment highlighting the top 10 campaigns.
    - Monthly trends visualized using line and bar charts.
    - Filters for campaigns, dates, and regions.
- Deployment:

  - Validate metrics and publish the dashboard for real-time stakeholder access.

# Challenges and Solutions
**Data Mapping**
- Challenge: Aligning external campaign data with internal revenue records.
- Solution: Establish a standardized naming convention and automate validation.
**Data Quality**
- Challenge: Inconsistent or incomplete data.
- Solution: Implement data cleaning and validation steps in the ETL process.
**Scalability**
- Challenge: Handling growing datasets as campaigns expand.
- Solution: Optimize data queries and use scalable extraction tools like Analytics Canvas.

# Technologies Used
- Data Integration:
  - Google Analytics (GA4)
  - Analytics Canvas
  - MariaDB (stored procedures)
- Analytics:
  -Tableau (dashboard creation and KPI calculations)
- Programming:
  - SQL for data transformation
  - Python (for additional automation)

# Outcome
- Automated Workflow: Integrated ad spend and revenue data with minimal manual intervention.
- Data-Driven Insights: Provided stakeholders with metrics to evaluate marketing effectiveness.
- Scalable Solution: Designed a system capable of handling growing campaign data.
![Ads yearly](https://github.com/user-attachments/assets/e5d6cf37-a734-447e-9e18-b6715a98f901)



