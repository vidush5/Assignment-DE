# Data Engineering Assignment: Kafka, Kafka Connect, and MySQL Integration

## Objective
The objective of this assignment is to set up a streaming pipeline using Apache Kafka and Kafka Connect on Docker. This pipeline will generate streaming data, process it, and store it in a MySQL database with updates reflecting as they occur.

## Pipeline Architecture
![Data Engineering Architecture](https://github.com/vidush5/Assignment-DE/blob/main/architecturede.JPG)

## Project Explanation
This project revolves around a streamlined data flow process facilitated by Kafka and Kafka Connect. Firstly, leverage a data generator to generate data. Next, utilizing Kafka Connect, this data is seamlessly published to a Kafka broker. Subsequently, subscribers, through topic subscription, access and read the generated data. Lastly, to ensure real-time updates by utilizing this data to update a MySQL table, facilitating efficient and synchronized data management. 

# Docker
Docker is a platform that streamlines software development by enabling developers to build, ship, and run applications in containers. These containers encapsulate all necessary components, ensuring consistent performance across diverse systems. Docker accelerates development cycles by simplifying deployment and scaling, reducing setup time and effort. Moreover, it facilitates collaboration among teams, enabling easy sharing and deployment of applications. In essence, Docker revolutionizes software development by offering a lightweight, efficient, and standardized approach to application packaging and deployment.

# Kafka 
Kafka is a distributed streaming platform designed to handle large volumes of real-time data efficiently. It provides a high-throughput, fault-tolerant system for publishing, subscribing to, and storing streams of records in real time. Kafka's architecture allows for horizontal scalability, enabling seamless handling of data streams across clusters of machines. It is widely used for building real-time data pipelines, event-driven architectures, and stream processing applications. 

# Kafka-Connect
Kafka Connect is a framework within Apache Kafka that enables scalable, reliable streaming data integration with external systems. It simplifies the development of data pipelines by providing a set of connectors for easily ingesting and exporting data between Kafka topics and various data sources or sinks

Quick Start
===========

* ``docker-compose up -d --build`` start all services

* Run ``docker-compose ps`` to see all services' states

* Login to connect instance and run ``curl -i -X POST -H "Accept:application/json" -H  "Content-Type:application/json" http://localhost:8083/connectors/ -d @datagen-config.json``


  

## Resources
- https://developer.confluent.io/tutorials/kafka-connect-datagen/kafka.html
- https://zendesk.engineering/create-a-test-data-generator-using-kafka-connect-f0a2419af76a
- https://medium.com/@gmtang.rocks/kafka-connect-an-easier-way-to-connect-messages-with-data-stores-84e24348d216
- https://github.com/xushiyan/kafka-connect-datagen/tree/0.1.0/example/quickstart










