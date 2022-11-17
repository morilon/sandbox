# sandbox is a dev environment for my projects.

It contains all the infrastructure necessary to run what I need.

## Environment Setup

```
# this will setup and you'll have everything up and running.
docker compose up -d --build
```

### If you need something specific or less servics, just start those instead.

```
# this will setup and you'll have everything up and running.
docker compose up -d --build kafka
# Will start up kafka and zookeeper.
```

## Important Info

Everything works, just remember to create your user before using it.

## Available Services

Name|Port|GUI Port|Other
---|---|---|---
Postgres|5432|---|access: dbadmin/dbpass
Mongo|27017|---|
Redis|6379|---|
Kafka|9092|---|
Kafka Zookeeper|2181|---|
RabbitMQ|5672|[15001](http://localhost:15001)|access: rmqadmin/rmqpass
Keycloak|10001|[10001](http://localhost:10001)|
Mailhog|1025|[15002](http://localhost:15002)|