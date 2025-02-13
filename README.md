# Realtime-Streaming-Data
## Realtime Streaming Data Process using Kafka, Airflow and Spark.

## Top contents:
+ Extract Random User data from https://randomuser.me/ API using **Apache Airflow** as Data Orchestration Tool.
+ Trigger **Kafka** Producer and Kafka Consumer on schedule to start streaming data.
+ Kafka Monitoring and Management using **Apache Zooker, Control Center** and **Confluent Schema Registry**.
+ Performing **Spark Master** and **Spark Worker** for streaming data.
+ **Apache Cassandra** as a Distributed Database.

## Prerequisites
1. Have your Docker installed on your computer, then check: docker -version and docker compose -version.
2. In your terminal, run docker compose up -d.
3. Trigger the user_automation task on Airflow Web UI.
4. Check if the Kafka topic has been created on Control Center.
5. In the terminal, run the command:
``` spark-submit --master spark://localhost:7077 spark_stream.py ```
to submit spark job.
6. Run the Cassandra cluster and do some stuff of SQL query (SELECT FROM).

## System Architecture
![image](https://github.com/user-attachments/assets/f326d1f3-72e0-42b0-810d-f7874a863c3a)

## How can I make this project more practical and better? :)
A lot can still be done:
+ Cloud composer for Airflow, Kafka and Spark (such as AWS Managed Service for Airflow, Kafka, EMR for Spark).
+ Data quality tests.
+ OLAP Operations with Data Warehouse for analytical purposes.
