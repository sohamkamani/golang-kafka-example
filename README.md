## Kafka Golang Example

Example code for my [blog post](https://sohamkamani.com/golang/working-with-kafka/).

Steps to run:

1. Clone this repository
2. Install dependencies : `go mod tidy && go mod vendor`
3. Make sure [Kafka is running](https://www.sohamkamani.com/blog/2017/11/22/how-to-install-and-run-kafka/), and change the value of `brokerAddress` to the address of you Kafka instance
4. Run the code : `go run main.go`

Another way to run if you don't want to install kafka locally:

1. Clone this repository
2. Install dependencies : `go mod tidy && go mod vendor`
3. `docker-compose up -d` to run kafka and zookeeper in docker
4. docker exec -it golang-kafka-example_kafka_1 kafka-topics.sh --create --bootstrap-server kafka:9092 --topic message-log --partitions 1 --replication-factor 1 to create topic
5. Run the code : `go run main.go`


> You can see how to install and run a Kafka cluster in my [other tutorial](https://www.sohamkamani.com/blog/2017/11/22/how-to-install-and-run-kafka/)
