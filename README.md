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




# [Project 2: Face Recognition-Based Attendance System for Higher Education Institution](https://github.com/phdamg/phdamg.github.io)

## **Project Overview**
This project was conducted for a higher education (HE) institution with tens of thousands of students, aiming to modernize and automate the attendance marking process. Traditional attendance methods, such as manually calling student names, are time-consuming and prone to errors or proxy attendance. To address these challenges, I developed a **face recognition-based attendance system**, which leverages biometric technology to ensure accuracy, speed, and efficiency.

The system uses face recognition techniques to identify and verify students in real-time, marking attendance seamlessly. This non-intrusive solution eliminates the need for manual intervention, reduces time overhead for faculty, and enhances the integrity of the attendance process.

---

## **Objectives**
- **Automate Attendance**:
  - Replace manual attendance marking with a robust, automated system using face recognition.
- **Enhance Efficiency**:
  - Minimize time spent on attendance in large classes, improving overall session efficiency.
- **Improve Accuracy**:
  - Mitigate errors and prevent proxy attendance through biometric verification.

---

## **Finalized Approach**
1. **Dataset Preparation**:
   - Compiled a dataset of labeled facial images for all students enrolled in the institution.
   - Ensured the dataset represents diverse facial expressions and angles for robust recognition.

2. **Face Encoding**:
   - Encoded facial features using the **face_recognition library**, achieving a 99.38% accuracy in face matching.

3. **Real-Time Detection**:
   - Integrated **Mediapipe**, a high-speed face detection framework, capable of detecting faces within 0.01 seconds.

4. **Face Identification**:
   - Leveraged **face_recognition** for 1:N matching to compare detected faces against the stored database.

5. **Attendance Logging**:
   - Stored the recognized student’s name, along with the timestamp, in a relational database for future retrieval and reporting.

6. **System Workflow**:
   - Detect a face in real-time using Mediapipe.
   - Identify the face using the encoded features in the database.
   - Log the student’s attendance details in the database automatically.

---

## **Technologies and Tools Used**
- **Face Detection**: Mediapipe for real-time, high-speed face detection.
- **Face Recognition**: Python's face_recognition library for high-accuracy identification.
- **Data Storage**: Relational database (MySQL) to store attendance records.
- **Programming Language**: Python for building the system's logic and integration.
- **Deployment Platform**: Flask or similar web frameworks for system accessibility.

---

## **Key Features**
- **Speed**:
  - Detects faces in real-time, reducing the time required to mark attendance to mere seconds.
- **Accuracy**:
  - Achieves a recognition accuracy of 99.38%, ensuring reliable identification.
- **Scalability**:
  - Capable of handling tens of thousands of students with minimal computational overhead.
- **Non-Intrusive**:
  - Uses facial recognition, eliminating the need for physical interaction with devices.

---

## **Impact**
- Reduced attendance marking time from ~5 minutes per session to just seconds, saving significant time across all sessions.
- Eliminated proxy attendance issues, improving trust and accountability in attendance records.
- Streamlined faculty workload, allowing them to focus more on teaching rather than administrative tasks.
- Established a scalable framework for future integrations, such as combining attendance data with academic performance analytics.

---

## **Next Steps**
- Integrate the system with the institution's Learning Management System (LMS) for seamless reporting.
- Enhance robustness by incorporating additional biometric features (e.g., iris or voice recognition).
- Deploy the system on the cloud for improved scalability and accessibility.

![image](https://user-images.githubusercontent.com/114836975/193611560-5423d7f7-76c1-4622-896e-ffa99c526c53.png)
![image](https://user-images.githubusercontent.com/114836975/193612294-a03fbda3-7796-4389-88aa-5a3795680ef2.png)<br/><br/><br/><br/><br/><br/>





