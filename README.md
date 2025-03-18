# 🎢 Real-Time Amusement Park Wait Times ETL Pipeline  

![Flow Chart](https://github.com/tanmay1501/Queue-time/blob/main/Data-flow.png)

![Dashboard](https://github.com/tanmay1501/Queue-time/blob/main/Dashboard.png)
## 📌 Project Overview  
This project builds an **end-to-end ETL pipeline** that automates the collection, transformation, and visualization of **real-time ride wait times** from **65 amusement parks across the USA**. It leverages **AWS Lambda, S3, Snowflake, and Streamlit** to provide continuously updated insights every **5 minutes**.  

## 🚀 Tech Stack  
- **Data Extraction:** AWS Lambda, Queue Time API  
- **Data Storage:** AWS S3  
- **Data Ingestion:** Snowpipe (Continuous Integration)  
- **Data Processing & Transformation:** Snowflake (Streams & Tasks)  
- **Visualization:** Streamlit Dashboard  
- **Automation:** AWS & Snowflake  

## 📊 Features  
✔ **Real-Time Data Updates:** Fetches live ride wait times every 5 minutes  
✔ **Automated ETL Pipeline:** Fully managed data ingestion, transformation, and enrichment with ZIP codes  
✔ **Scalable Cloud Architecture:** AWS + Snowflake integration ensures reliability and scalability  
✔ **Interactive Dashboard:** Displays **live wait times** for better ride planning and queue monitoring  

## 🔧 Project Workflow  
1️⃣ **Data Extraction:**  
   - AWS Lambda calls the **Queue Time API** to fetch JSON ride wait times  
   - Stores raw data in **AWS S3**  

2️⃣ **Data Ingestion & Processing:**  
   - Snowpipe **automatically** loads data from S3 to Snowflake  
   - Data is **flattened** and **enriched** with ZIP codes  
   - Snowflake **Streams & Tasks** handle automated transformations  

3️⃣ **Visualization & Analysis:**  
   - A **Streamlit Dashboard** displays real-time wait times dynamically  

## 📂 Repository Structure  
```plaintext
📦 amusement-park-wait-times-etl  
 ┣ 📂 lambda_function/         # AWS Lambda function for API calls  
 ┣ 📂 data/                    # Sample JSON data  
 ┣ 📂 snowflake_scripts/       # SQL scripts for data transformation  
 ┣ 📂 streamlit_dashboard/     # Streamlit app code  
 ┣ 📜 requirements.txt         # Dependencies for Streamlit & Snowflake  
 ┣ 📜 README.md                # Project Documentation  
