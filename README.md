# 🌤️ Weather Data ETL Pipeline with Apache Airflow and AWS S3

![ETL-Pipeline](https://github.com/kebishaa/Build-and-automate-Python-ETL-Pipeline/blob/main/screenshot/photo_2025-06-10_13-43-42.jpg?raw=true)!

🌦️ Build and Automate a Python ETL Pipeline with Airflow
This project extracts weather data from an API, transforms it, and loads it into an Amazon S3 bucket. The ETL process is orchestrated using Apache Airflow.

🚀 Getting Started
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/kebishaa/Build-and-automate-Python-ETL-Pipeline
cd weather-etl-airflow
2. Install Python and Create Virtual Environment
bash
Copy
Edit
sudo apt update
sudo apt install python3-pip python3.10-venv -y
python3 -m venv airflow_venv
source airflow_venv/bin/activate
