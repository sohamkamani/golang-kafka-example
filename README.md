## Kafka Golang Example

Example code for my [blog post](https://sohamkamani.com/golang/working-with-kafka/).

Steps to run:

1. Clone this repository
2. Install dependencies : `go mod tidy && go mod vendor`
3. Make sure [Kafka is running](https://www.sohamkamani.com/blog/2017/11/22/how-to-install-and-run-kafka/), and change the value of `brokerAddress` to the address of you Kafka instance
4. Run the code : `go run main.go`
