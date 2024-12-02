# Dr Abdulrahman Mahmoud's portfolio


# [Project 1: Data Warehousing for Aircall data](https://github.com/phdamg/Aircall)

# Project Overview
The Patient Advisory Team (PAT) at the company advises patients on healthcare products and services through phone calls facilitated by **Aircall**, a cloud-based telephony platform. The board tasked me with building a **data warehouse** to centralize, organize, and analyze PAT performance data. The data warehouse provides insights into key metrics such as call duration, advisor availability, and patient engagement, enabling management to evaluate team performance and operational efficiency.

# Objectives
- **Data Centralization**: Integrate raw data from the Aircall API into a structured data warehouse for analysis.
- **Data Modeling**: Design a scalable schema to store and query key metrics, including:
  - Call Logs
  - Advisor Availability
  - Patient Interaction and Engagement
- **Performance Monitoring**: Enable analysis of team effectiveness using metrics such as:
  - Total Calls
  - Average Call Duration
  - Advisor Utilization Rates
  - Message Delivery Metrics
- **Visualization**: Provide actionable insights through interactive Tableau dashboards tailored for non-technical stakeholders.

# Project Workflow
- **Data Integration**:
  - Connected to the Aircall API to extract datasets such as call logs, availability, and engagement data.
  - Automated data ingestion pipelines to retrieve and store the data into MariaDB.

- **Data Warehouse Design**:
  - Designed a **star schema** with fact and dimension tables to facilitate efficient querying and reporting:
    - Fact Table: Call logs with metrics like duration and engagement.
    - Dimension Tables: Advisors, time, and interaction categories.
  - Normalized data to reduce redundancy and ensure scalability.

- **ETL Pipeline Development**:
  - Built an ETL (Extract, Transform, Load) process to:
    - Extract raw data from the Aircall API.
    - Transform data to align with the data warehouse schema.
    - Load processed data into MariaDB tables.

- **Data Analysis**:
  - Queried the data warehouse to calculate performance metrics:
    - Total calls made by each advisor.
    - Average call duration and time of day trends.
    - Advisor availability and utilization rates.
    - Patient interaction metrics like message success rates.

- **Dashboard Creation**:
  - Designed a Tableau dashboard to visualize:
    - Team and individual performance.
    - Trends in call activity and advisor availability.
    - Metrics for patient engagement and outcomes.

# Challenges and Solutions
**API Data Integration**
- **Challenge**: Complex, nested data structures from the Aircall API.
- **Solution**: Flattened data structures during the ETL process to fit the data warehouse schema.

**Schema Design**
- **Challenge**: Balancing schema flexibility with query performance.
- **Solution**: Implemented a star schema to support both complex analysis and scalability.

**Data Quality**
- **Challenge**: Inconsistent and missing data from the source.
- **Solution**: Added validation checks and transformations in the ETL pipeline to ensure data integrity.

**Stakeholder Reporting**
- **Challenge**: Presenting technical insights in a non-technical format.
- **Solution**: Created simplified Tableau dashboards with clear visualizations and tooltips for contextual understanding.

# Technologies Used
- **Data Integration**:
  - Aircall API for data extraction.
- **Data Warehouse**:
  - MariaDB for schema design and data storage.
- **ETL Pipeline**:
  - SQL for data transformation and loading.
  - Python (for automation scripts).
- **Data Visualization**:
  - Tableau for interactive dashboards.

# Outcome
- **Centralized Data Warehouse**: Built a robust data warehouse to store and manage PAT performance data.
- **Actionable Insights**: Enabled management to track advisor performance, operational efficiency, and patient engagement.
- **Scalable Solution**: Designed a schema capable of handling growing data volumes and new performance metrics.
- 
![T1511_model](https://github.com/user-attachments/assets/3d3bfcc9-aebc-4497-9c99-0ea658908853)<br/><br/><br/><br/><br/><br/>

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

![Ads_yearly](https://github.com/user-attachments/assets/a3d55f84-845e-4420-99a4-a249c441829a)



# [Project 3: Facial recognition based attendance monitoring system](https://github.com/phdamg/phdamg.github.io)

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





