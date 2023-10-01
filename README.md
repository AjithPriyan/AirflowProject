# AirflowProject
In this project, I will create an ETL process for extracting data and wrap the whole thing as a data pipeline using Airflow and Docker.

The ETL process will extract data from API, the extracted data is stored in XCOM(Connection between two tasks), then data is temporarily stored in CSV file and finally transform it and load it to a PostgreSQL database. It have an automated process that constantly feeds the PostgreSQL database with data. Every 2 minutes, the ETL process will load an updated batch of API data.

# Project Details
Airflow Project, which consists of
1. Setting up Airflow Architecture
2. 1st Dag — Check if API is available
3. 2nd Dag — Create a table
4. 3rd Dag — Extract
5. 4th Dag — Transform
6. 5th Dag — Load
7. Query data in the pgAdmin UI
