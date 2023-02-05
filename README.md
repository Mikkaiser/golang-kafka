### How can I run this project?

Run `docker compose up -d` to setup all containers:

- Go container with [librdkafka](https://github.com/confluentinc/librdkafka) installed;
- Zookeeper Kafka metadata manager;
- The Kafka;
- Control Center to get an interface to help manage the Kafka's traffic.

Type `docker compose exec goapp bash` to enter in Go container.

go to `/cmd/producer` to and run `go run main.go` to run the producer, and the same into `/cmd/consumer` to run the consumer and log the producer's messages.
