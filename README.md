# TypeScript KafkaJS

## Simple Producer & Client example in KafkaJS

### How to run:

#### Step 1: Setup Kafka and Zookeeper

```
docker-compose up -d
```

#### Step 2: Create Kafka topic from inside broker

```
docker exec broker \
kafka-topics --bootstrap-server broker:9092 \
             --create \
             --topic test-topic
```

#### Step 3: Run Producer

```
npx ts-node src/producer.ts
```

#### Step 4: Run Consumer

In another terminal:

```
npx ts-node src/consumer.ts
```

Customization of: https://github.com/maddymanu/TypeScript-KafkaJS-Example
