# Kafka Nodejs Example

This is a simple example of how to use Kafka with Nodejs. It uses the [kafkajs](https://kafka.js.org/) library to interact with Kafka. 

## Requirements

- Docker
- Docker-compose
- Nodejs

## How to run

1. Install docker and docker-compose

2. Run the following command to start the kafka cluster

```bash
docker compose up -d
```

3. Run the following command to start the producer

```bash
node producer.js
```

4. Run the following command to start the consumer

```bash
node consumer.js
```

5. You should see the messages being sent and received in the terminal.

```bash
Produced event to topic purchases: key = awalther   value = batteries
Produced event to topic purchases: key = awalther   value = batteries
Produced event to topic purchases: key = jbernard   value = t-shirts
Produced event to topic purchases: key = eabara     value = book
Produced event to topic purchases: key = htanaka    value = batteries
Produced event to topic purchases: key = jbernard   value = gift card
Produced event to topic purchases: key = htanaka    value = t-shirts
Produced event to topic purchases: key = htanaka    value = gift card
Produced event to topic purchases: key = jbernard   value = alarm clock
Produced event to topic purchases: key = eabara     value = gift card
````

```bash
Consumed event from topic purchases: key = jbernard   value = t-shirts
Consumed event from topic purchases: key = jbernard   value = alarm clock
Consumed event from topic purchases: key = jbernard   value = book
Consumed event from topic purchases: key = jbernard   value = batteries
Consumed event from topic purchases: key = jsmith     value = alarm clock
Consumed event from topic purchases: key = jsmith     value = book
Consumed event from topic purchases: key = sgarcia    value = batteries
Consumed event from topic purchases: key = jsmith     value = batteries
Consumed event from topic purchases: key = awalther   value = batteries
Consumed event from topic purchases: key = awalther   value = batteries
Consumed event from topic purchases: key = jbernard   value = t-shirts
Consumed event from topic purchases: key = eabara     value = book
Consumed event from topic purchases: key = htanaka    value = batteries
Consumed event from topic purchases: key = jbernard   value = gift card
Consumed event from topic purchases: key = htanaka    value = t-shirts
Consumed event from topic purchases: key = htanaka    value = gift card
Consumed event from topic purchases: key = jbernard   value = alarm clock
Consumed event from topic purchases: key = eabara     value = gift card
```
