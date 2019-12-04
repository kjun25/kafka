# kafka
Kafka Producer/Consumer 
## zookeeper-server
```sh
bin/zookeeper-server-start.sh config/zookeeper.properties
```
## kafka-server
```sh
bin/kafka-server-start.sh config/server.properties
```
## kafka-command
```sh
bin/kafka-topics.sh --list --zookeeper localhost:2181
```  
```sh
bin/kafka-topics.sh --delete --zookeeper localhost:2181
```  
```sh
bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic TOPIC_NAME
```
```sh
bin/kafka-topics.sh --describe --zookeeper localhost:2181 --topic TOPIC_NAME
```
## kafka-console
```sh
bin/kafka-console-producer.sh --broker-list localhost:9092 --topic TOPIC_NAME
```  
```sh
bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic TOPIC_NAME --from-beginning
```  
