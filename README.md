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

**Medium Article:** https://medium.com/@rutvij3007/building-a-data-pipeline-my-journey-in-data-engineering-during-a-data-science-bootcamp-cb0d43ebbc3#id_token=eyJhbGciOiJSUzI1NiIsImtpZCI6IjFmNDBmMGE4ZWYzZDg4MDk3OGRjODJmMjVjM2VjMzE3YzZhNWI3ODEiLCJ0eXAiOiJKV1QifQ.eyJpc3MiOiJodHRwczovL2FjY291bnRzLmdvb2dsZS5jb20iLCJhenAiOiIyMTYyOTYwMzU4MzQtazFrNnFlMDYwczJ0cDJhMmphbTRsamRjbXMwMHN0dGcuYXBwcy5nb29nbGV1c2VyY29udGVudC5jb20iLCJhdWQiOiIyMTYyOTYwMzU4MzQtazFrNnFlMDYwczJ0cDJhMmphbTRsamRjbXMwMHN0dGcuYXBwcy5nb29nbGV1c2VyY29udGVudC5jb20iLCJzdWIiOiIxMDgwOTkxMjIyOTI5ODAzNTAzMDgiLCJlbWFpbCI6InJ1dHZpajMwMDdAZ21haWwuY29tIiwiZW1haWxfdmVyaWZpZWQiOnRydWUsIm5iZiI6MTcwNTMxNDc2OSwibmFtZSI6IlJ1dHZpaiBQYXRlbCIsInBpY3R1cmUiOiJodHRwczovL2xoMy5nb29nbGV1c2VyY29udGVudC5jb20vYS9BQ2c4b2NKT0ZkWUFBM21udlNSa2dtMXdsYVAyUFZyZ3JKcjI5SmVjdWZNZ0tuQ1lyY0k9czk2LWMiLCJnaXZlbl9uYW1lIjoiUnV0dmlqIiwiZmFtaWx5X25hbWUiOiJQYXRlbCIsImxvY2FsZSI6ImVuIiwiaWF0IjoxNzA1MzE1MDY5LCJleHAiOjE3MDUzMTg2NjksImp0aSI6ImIxM2JiYWFhMzdjZTM0ZGZmNTk2ZmM1MjNkOGY5YWI1MTRlMjAzNDUifQ.MLLjOM3hwYq9VLcev9WrEHos-KyG5g2kJjb5cLBylbXbU7Fzo34KHcjGg8CcW8YhKw5mJq_UwhvpEYI5CIuEUEHGVWnhKvx3RiRR7IT3RDOLU6duAkqgkNK2_BVUMaV2F7gEjHXQpd3zGoKZLF5SUopTnTt70dfCu-2GDWDUWM7LZVtMkJUkeRDqQehc-5zK_6-FakY-0SSFi14Mlaa1jXIEjngODZGMb4F9C7GqrvQy1DXUndIDfT8rEImebecnSoONG5ybD2spsmOLDK0GbxAkVisMoRd7JtSvASqUrGN9gRZZnQLRM89fv-25w6KJjv35gEStqkLQoB67QfUzAw

**Questions or Suggestions:** Feel free to reach out. Happy coding!
