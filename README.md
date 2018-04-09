## Source
- https://medium.com/@shijuvar/building-high-performance-apis-in-go-using-grpc-and-protocol-buffers-2eda5b80771b (gRPC Tutorial)
- https://gist.github.com/skyrocknroll/8f7c9d2f60bebbee717e82993efb0363 (Install Proto3)

## Setup
- Get Dependencies
    - go get -u github.com/golang/protobuf/proto
    - go get -u github.com/golang/protobuf/protoc-gen-go
    - go get google.golang.org/grpc


- Install protobuf 3 on ubuntu 16 (Source: https://gist.github.com/skyrocknroll/8f7c9d2f60bebbee717e82993efb0363)

- Generate .pb.go file 
    - protoc -I customer/ customer/customer.proto --go_out=plugins=grpc:customer

## How to Run
1. cd server, go run main.go
2. cd client, go run main.go