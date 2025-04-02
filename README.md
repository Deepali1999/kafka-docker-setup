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
