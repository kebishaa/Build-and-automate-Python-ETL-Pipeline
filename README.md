# 🌤️ Weather Data ETL Pipeline with Apache Airflow and AWS S3

![ETL-Pipeline](https://github.com/kebishaa/Build-and-automate-Python-ETL-Pipeline/blob/main/screenshot/photo_2025-06-10_13-43-42.jpg?raw=true)!

This project extracts weather data from an API, transforms it, and loads it into an Amazon S3 bucket. The ETL process is orchestrated using Apache Airflow.

🔧 Project Features

● Extracts real-time weather data from an API.

● Cleans and transforms the data using pandas.

● Saves the transformed data to AWS S3 in CSV format.

● Orchestrates and automates the pipeline using Apache Airflow.

🚀 Getting Started
1. Clone the Repository
   ```bash
   git clone https://github.com/kebishaa/Build-and-automate-Python-ETL-Pipeline
   cd weather-etl-airflow
2. Install Python and Create Virtual Environment
    ```bash
    sudo apt update
   sudo apt install python3-pip python3.10-venv -y
   python3 -m venv airflow_venv
   source airflow_venv/bin/activate
3. Install Dependencies
    ```bash
    pip install --upgrade pip
    pip install -r requirements.txt
4. Install and Configure AWS CLI
     ```bash
      sudo apt install awscli -y
      aws configure
5. Start Airflow
    ```bash
    airflow standalone
This will initialize Airflow and start the webserver and scheduler.
Default username: admin, password: auto-generated in terminal



✅ Prerequisites
Python 3.10+

AWS Account with S3 bucket access

Apache Airflow 2.7+ (use standalone for local setup)

Internet access to call the weather API

🧪 Testing
   You can manually run the DAG from the Airflow web UI or trigger it via CLI 
 ```bash
 airflow dags trigger weather_etl_dag

