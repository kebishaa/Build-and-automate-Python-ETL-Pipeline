# 🌤️ Weather Data ETL Pipeline with Apache Airflow and AWS S3

![ETL-Pipeline](https://github.com/kebishaa/Build-and-automate-Python-ETL-Pipeline/blob/main/screenshot/photo_2025-06-10_13-43-42.jpg?raw=true)!

##This project is an automated ETL (Extract, Transform, Load) pipeline built in Python that fetches weather data from a public API, transforms it using pandas, and loads it into an Amazon S3 bucket. Apache Airflow is used to orchestrate and schedule the ETL process.


🔧 Project Features
Extracts real-time weather data from an API.

Cleans and transforms the data using pandas.

Saves the transformed data to AWS S3 in CSV format.

Orchestrates and automates the pipeline using Apache Airflow.

📁 Project Structure

⚙️ Setup Instructions
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
