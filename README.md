## DEMO KAFKA
- Run Zookeeper Server
  > ./bin/zookeeper-server-start.sh config/zookeeper.properties
- Run Kafka Server
  > ./bin/kafka-server-start.sh config/server.properties
- Create Kafka Topics (Create 3 Partitions)
  > ./bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 3 --topic topic-java-lagi
- Show List Kafka Topics
  > ./bin/kafka-topics.sh --list --zookeeper localhost:2181