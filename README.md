# kafka-docker-setup

- clone this repository
- Move inside the cloned directory and execute below commands


```
docker compose up -d

```

- Now once the container is up, use the following command to entre the kafka shell running inside the container.
- ```
  docker exec -it -w /opt/kafka/bin broker sh
  ```
- To Add a topic in Kafka,
```
./kafka-topics.sh --create --topic sample-topic --bootstrap-server broker:29092
```
- To start consumer on a topic,
```
./kafka-console-consumer.sh --topic sample-topic --from-beginning --bootstrap-server broker:29092
```
- To produce the data in the topic,
```
./kafka-console-producer.sh --topic sample-topic --bootstrap-server broker:29092
```
