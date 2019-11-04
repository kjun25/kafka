# kafka
Kafka Producer/Consumer 
# zookeeper-server
bin/zookeeper-server-start.sh config/zookeeper.properties
# kafka-server
bin/kafka-server-start.sh config.server.properties
# kafka-command
bin/kafka-topics.sh --list --zookeeper localhost:2181
bin/kafka-topics.sh --delete --zookeeper localhost:2181
bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic TOPIC_NAME
# kafka-console
bin/kafka-console-producer.sh --broker-list localhost:9092 --topic TOPIC_NAME
bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic TOPIC_NAME --from-beginning
