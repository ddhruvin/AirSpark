# Realtime Data Streaming | AirSpark

## Table of Contents
- [Introduction](#introduction)
- [System Architecture](#system-architecture)
- [Screenshots](#screenshots)
- [Technologies](#technologies)
- [Replicate results](#replicate-results)
## Introduction

This project serves as a comprehensive guide to building an end-to-end data engineering pipeline. It covers each stage from data ingestion to processing and finally to storage, utilizing a robust tech stack that includes Apache Airflow, Python, Apache Kafka, Apache Zookeeper, Apache Spark, and Cassandra. Everything is containerized using Docker for ease of deployment and scalability.

## System Architecture

![System Architecture](https://github.com/airscholar/e2e-data-engineering/blob/main/Data%20engineering%20architecture.png)

The project is designed with the following components:

- **Data Source**: We use `randomuser.me` API to generate random user data for our pipeline.
- **Apache Airflow**: Responsible for orchestrating the pipeline and storing fetched data in a PostgreSQL database.
- **Apache Kafka and Zookeeper**: Used for streaming data from PostgreSQL to the processing engine.
- **Control Center and Schema Registry**: Helps in monitoring and schema management of our Kafka streams.
- **Apache Spark**: For data processing with its master and worker nodes.
- **Cassandra**: Where the processed data will be stored.

## Screenshots
![image](https://github.com/user-attachments/assets/72c46103-4d78-42ef-bc79-abdf71c24b54)
![image](https://github.com/user-attachments/assets/11ccc73b-8d5b-4a0e-8fc3-8b5515de714e)
![image](https://github.com/user-attachments/assets/5d8cbe73-e645-4052-ba4c-c16ed4f24cdc)




## Technologies

- Apache Airflow
- Python
- Apache Kafka
- Apache Zookeeper
- Apache Spark
- Cassandra
- PostgreSQL
- Docker

## Replicate results

1. Clone the repository:
    ```bash
    git clone https://github.com/airscholar/e2e-data-engineering.git
    ```

2. Navigate to the project directory:
    ```bash
    cd e2e-data-engineering
    ```

3. Run Docker Compose to spin up the services:
    ```bash
    docker-compose up
    ```
