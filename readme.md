# Kafka Commands

## config file changes
* C:\kafka\config\zookeeper.properties
* C:\kafka\config\server.properties


## start zookeper & kakfa server
* C:\kafka\bin\windows\zookeeper-server-start.bat C:\kafka\config\zookeeper.properties
* C:\kafka\bin\windows\kafka-server-start.bat C:\kafka\config\server.properties

## create topic
* C:\kafka\bin\windows\kafka-topics.bat --create --bootstrap-server localhost:9092 --replication-factor 1 --partition 1 --topic test

## list topics
* C:\kafka\bin\windows\kafka-topics.bat --list --bootstrap-server localhost:9092

## producer terminal
* C:\kafka\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic test

## consumer terminal
* C:\kafka\bin\windows\kafka-console-consumer.bat --topic test --bootstrap-server localhost:9092 --from-beginning


## Sample Data
* {"Name: "John", "Age":"31", "Gender":"Male"}
* {"Name: "Emma", "Age":"27", "Gender":"Female"}
* {"Name: "Ronald", "Age":"17", "Gender":"Male"}