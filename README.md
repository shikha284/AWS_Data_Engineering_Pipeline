# AWS_Data_Engineering_Pipeline

In this project, we are working on **Cloud Analytics** and **Data Warehouse Implementation** by building a data pipeline to analyze archival and real-time weather data and gather useful insights from this data. Key weather indicators such as temperature, precipitation, wind speed, and pressure play pivotal roles in various sectors, including agriculture, travel, and supply chain management. By delving into the analysis of temperature trends spanning multiple years, valuable insights can be extracted and visualized to benefit different industries. The escalating global temperatures have become a cause for widespread apprehension. 🌍

### 🌐 Data Sources

Global Historical Climatology Network (GHCN) data from the National Oceanic and Atmospheric Administration (NOAA) website has been utilized for the purpose of analysis and building a data pipeline using Amazon Web Services (AWS). Data is directly sourced from the open data registry on AWS, courtesy of the National Oceanic and Atmospheric Administration (NOAA). 

Dataset links:
- [NOAA GHCN Data on AWS](https://registry.opendata.aws/noaa-ghcn/)
- [NOAA GHCN PDS](https://noaa-ghcn-pds.s3.amazonaws.com/index.html)

### ☁️ Cloud Architecture

![image](https://github.com/user-attachments/assets/6215cc69-7b1a-4e17-bacc-9a4e38281cbd)

### ⚙️ ETL Jobs

- 📥 Supplementary Data Ingestion Glue Job
- 🗄️ Archived Data Ingestion Glue Job
- ⏱️ Realtime Data Ingestion Glue Job
- 🗃️ Supplementary Data Redshift Ingestion Glue Job

### 🗃️ Data Modeling

OLAP (Online Analytical Processing) database was implemented using a snowflake schema with fact and dimensions tables. A Snowflake Schema is a database schema commonly employed in data warehousing, particularly when designing structures for large-scale analytical databases. The Snowflake Schema takes normalization a step further, resulting in a more intricate, normalized architecture. ❄️

![image](https://github.com/user-attachments/assets/530b2e55-6363-4a4c-8c07-580456803251)

### ⏱️ Apache Airflow

Different glue jobs were orchestrated using two data pipelines:

1. **Real-Time Data Pipeline**

   ![image](https://github.com/user-attachments/assets/cc5e2594-1e49-4bdd-9cdc-f4d843d0113c)

2. **Archive Data Pipeline**

   ![image](https://github.com/user-attachments/assets/6ff7ab78-052d-4891-9312-fd65f98b9b3f)

### 📊 Data Analytics and Visualizations

1. **Average Weather Parameters by Year and Month**

   ![image](https://github.com/user-attachments/assets/47041e83-f828-4435-b5a2-cf9da4ac09a0)

2. **Comparison of Monthly Precipitation Values**

   ![image](https://github.com/user-attachments/assets/d325ed35-fed5-46e8-9d59-1bd87295228f)

3. **Year-wise Snowfall**

   ![image](https://github.com/user-attachments/assets/eb9d8816-6d8b-4834-b69b-609e168994d1)

4. **Weather Report**

   ![image](https://github.com/user-attachments/assets/b0668dae-ac13-47e8-ae75-a044c29e0e4a)

### 🧠 AWS SageMaker

The XGBoost Algorithm was used to train 5 different regression models to predict maximum and minimum temperature, precipitation, snowfall, and snow depth. 🌨️
