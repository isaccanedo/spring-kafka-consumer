# spring-kafka-consumer
Exemplo de consumidor Kafka construído com Spring Kafka

## Iniciando Zookeeper e Kafka

```
docker-compose up -d
```


## Running the consumer app

```
mvn spring-boot:run
```


## Producing sample data using kafka-console-producer

```
kafka-console-producer \
  --bootstrap-server localhost:29092 \
  --topic my-topic \
  --property parse.key=true \
  --property key.separator=":"
this-is-the-key:this-is-the-value
```
