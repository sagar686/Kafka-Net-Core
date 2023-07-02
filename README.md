# Kafka-Net-Core
C# client applications which produce and consume messages from an Apache Kafka® cluster.

Reference Link:
https://developer.confluent.io/get-started/dotnet/#introduction

**Steps to follow:**
1. Install Kafka on local docker
   
docker compose up -d
![image](https://github.com/sagar686/Kafka-Net-Core/assets/32801172/edaab0a6-0f2d-425e-a7f9-6b55807c7604)![image](https://github.com/sagar686/Kafka-Net-Core/assets/32801172/a448b8e6-9903-4925-9efc-15e99c80ce05)



2. Create Topics
   
   docker compose exec broker kafka-topics --create --topic purchases --bootstrap-server localhost:9092 --replication-factor 1 --partitions 1
![image](https://github.com/sagar686/Kafka-Net-Core/assets/32801172/391e6acb-00d7-44c0-aaa6-a4fa51722f33)

3. List Topics

   kafka-topics --list --bootstrap-server localhost:9092
 ![image](https://github.com/sagar686/Kafka-Net-Core/assets/32801172/ef90b5f6-4d95-4b33-a277-50ce882d4b8d)

4. Run producer and consumer console apps.
   
   ![image](https://github.com/sagar686/Kafka-Net-Core/assets/32801172/b700cf56-c0ad-4ba2-a4e6-070d415f756d)
