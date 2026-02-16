# Kafka Stock Cloud Simulation
Stock Simulation with Kafka Streams

## Description

The project uses t2.micro machine on AWS to simulate stock market flow. Each event is was created as a JSON file from existing dataset. The streamed data was analyzed in Crawler after being uploaded to S3 bucket which creates AWS Glue Data Catalog. This process allows to effectively utilize Amazon Athena. 

## Steps

The configurations are set up in kafka-producer and kafka-consumer. 
The process involves:
- Creating t2.micro instance
- downloading actual versions of kafka and Java on instance
- Accessing data on public IPv4 server
- starting zookeeper and kafka server
- starting producer and consumer on separate shells