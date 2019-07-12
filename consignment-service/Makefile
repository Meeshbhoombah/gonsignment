
build:
	protoc ./proto/consignment.proto --go_out=plugins=grpc:/Users/meeshbhoombah/go/src/github.com/microservices-container-tutorial/consignment-service/.
	GOOS=linux GOARCH=amd64 go build
	docker build -t consignment-service .

run:
	docker run -p 50051:50051 consignment-service

