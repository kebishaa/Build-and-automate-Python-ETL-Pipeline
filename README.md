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

This will initialize Airflow and start the webserver and scheduler. Default username: admin, password: auto-generated in terminal.

🔁 DAG Overview
Schedule: Daily (configurable)

Tasks:

extract_task: Pulls weather data from API

transform_task: Cleans and formats the data

load_task: Uploads data to your S3 bucket

✅ Prerequisites
Python 3.10+

AWS Account with S3 bucket access

Airflow 2.7+ (use standalone for local setup)

Internet access to call the weather API

🧪 Testing
You can manually run the DAG from the Airflow web UI or trigger it via CLI:
```bash
airflow dags trigger weather_etl_dag
🤝 Contributing
Feel free to fork this repo and submit pull requests. All contributions are welcome!

📜 License
This project is licensed under the MIT License. See the LICENSE file for details.

🙋‍♂️ Author
Kibatu Mezgebu – LinkedIn | Email | Addis Ababa, Ethiopia
