# 🌩 Deadly & Damaging Storm Events Data Pipeline

## 📌 Project Overview

This project involved designing and implementing an end-to-end cloud-based big data pipeline to analyze historical and real-time U.S. storm events.

The objective was to simulate a real-world engagement with a disaster relief organization to identify high-risk regions, analyze storm impact trends, and support predictive disaster preparedness planning.

---

## 🎯 Business Objective

Build a scalable data pipeline capable of:

- Identifying U.S. regions most vulnerable to severe storms
- Analyzing injuries, deaths, and property damage trends
- Monitoring real-time alert severity and urgency
- Forecasting potential storm damage for 2025
- Supporting data-driven disaster response planning

---

## 📊 Data Sources

### 1️⃣ Historical (Static) Dataset
- Source: NOAA Storm Events Database
- Time Range: 1950–2024
- ~2.9 million records
- 50+ structured features
- Includes storm type, injuries, deaths, property damage, crop damage

### 2️⃣ Streaming (Live) Dataset
- Source: National Weather Service (NWS) API
- Collection Date: April 20, 2025
- Semi-structured real-time alert data
- Includes severity, urgency, response type, headline text, issue & expiry times

---

## 🏗 Architecture & Workflow

Data Collection (Python APIs)  
→ Data Cleaning & Transformation (OpenRefine)  
→ Cloud Storage (Google Cloud Storage)  
→ Distributed Processing (Google Cloud Dataproc)  
→ Querying (Apache Hive & Spark SQL)  
→ Analytics & Visualization (BigQuery)  
→ Machine Learning Forecasting (BigQuery ML)

---

## 🛠 Technologies Used

- Python (API ingestion)
- OpenRefine (ETL & data cleaning)
- Google Cloud Storage (GCS)
- Google Cloud Dataproc
- Apache Hive
- Apache Spark (Spark SQL)
- BigQuery
- BigQuery ML
- IAM role-based access control

---

## 👩‍💻 My Contributions

- Transferred refined streaming dataset from GCS to HDFS
- Created structured Hive and Spark tables for distributed analysis
- Wrote and executed Spark SQL queries on streaming alert data
- Performed large-scale distributed aggregations on severity and urgency patterns
- Conducted word frequency analysis on alert headlines (basic NLP)
- Measured alert issue-to-expiration timing patterns
- Contributed to Apache Spark vs Hive performance benchmarking
- Interpreted analytical findings for disaster preparedness recommendations

---

## 🔍 Key Analyses Performed

- Storm event frequency by state and event type
- Total property and crop damage aggregation
- Injury and death impact analysis by region
- Daily alert distribution by severity and urgency
- Percentage distribution of alert categories
- Keyword extraction from alert headlines
- Spark vs Hive distributed performance comparison
- 2025 property damage forecasting using historical patterns

---

## 🤖 Machine Learning (Bonus Work)

Used BigQuery ML to:

- Forecast 2025 property damage trends
- Generate upper and lower prediction bounds
- Support proactive disaster preparedness planning

---

## 📈 Key Findings

- Texas, Kansas, and Oklahoma identified as highest-risk states
- Tornadoes and severe thunderstorms caused the highest long-term damage
- Inconsistencies found in alert severity and urgency labeling
- Apache Spark demonstrated faster distributed query performance than Hive
- Forecast suggests an upward trend in property damage for 2025

---

## 🚀 Business Impact

This scalable cloud-based pipeline demonstrates how:

- Historical + real-time integration improves situational awareness
- Distributed computing accelerates disaster analytics
- Predictive modeling supports proactive resource allocation
- Cloud infrastructure enhances emergency response planning

---

## 🤝 Team Collaboration

This was a group academic project completed at the University of North Texas for ADTA 5240 – Harvesting, Storing & Retrieving Data.

Full team details are included in the attached project report and presentation.

---

## 📎 Documentation

- 📄 [Full Technical Report (PDF)](./Strom%20data/docs/Storm_Data_Pipeline_Report.pdf)
- 📊 [Project Presentation (PPTX)]('./Strom data/Presentation_docs:Storm_Data_Pipeline_Report.pptx')

Both documents are available in this repository.

---

## 🔮 Future Improvements

- Integrate additional cyclone datasets
- Develop real-time automated monitoring dashboards
- Implement advanced NLP for alert message analysis
- Enhance predictive models with geospatial risk scoring
