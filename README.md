# Project-4-Data-Engineering

## Project Overview
This repository contains the code and resources for an automated data pipeline project developed during the Data Science Bootcamp at WBS Coding School. The goal is to create an efficient and scalable data pipeline for predicting e-scooter movement in the context of GANS, an e-scooter-sharing system.

### Components

1. **Data Collection:**
    - Utilizes web scraping and APIs to gather relevant data.
    - Web scraping with Python's Beautiful Soup for demographical data from Wikipedia.
    - APIs used: OpenWeather and Rapid API's Aerodatabox API for weather and flight data.

2. **Data Storage:**
    - MySQL chosen as the database management system.
    - Database schema designed to accommodate various data types and relationships.
    - SQLAlchemy used for data ingestion and interaction between Python and MySQL.

3. **Pipeline to the Cloud:**
    - Transitioned to the cloud using Amazon Web Services (AWS).
    - Amazon RDS MySQL instance set up for the cloud-based database.
    - AWS Lambda functions execute data collection and storage scripts in the cloud.

4. **Pipeline Automation:**
    - Automation achieved with AWS CloudWatch to schedule periodic triggers for Lambda functions.
    - Ensures automatic data collection at specified intervals for up-to-date information.

### Repository Structure

- **data_collection:** Code for web scraping and API data collection.
- **data_storage:** Code for MySQL database connection and table creation.
- **pipeline_aws:** Code and configuration files for deploying the data pipeline to AWS.
- **README.md:** Overview of the project and instructions for running the code.

### Prerequisites

- Weather API (5-day forecast) and AeroDataBox API keys required.
- AWS account for cloud deployment.

**WARNING:** Be cautious about AWS costs. Free tier options available, but costs may occur.

### Getting Started

1. Clone this repository to your local machine.
2. Install dependencies with `pip install -r requirements.txt`.
3. Modify code files as needed (update API keys, adjust data collection parameters).
4. Import data to the created database.
5. Create AWS Lambda layers with provided ARNs.
6. Run code locally by executing relevant scripts.
7. Set up a CloudWatch event schedule (tutorial link provided).

### Conclusion

This project demonstrates the power of data pipeline automation using MySQL, Python, and AWS. Explore the code and adapt it to your projects or use cases.

**Questions or Suggestions:** Feel free to reach out. Happy coding!
