# Simple gRPC Example

## Step 1:
Create a proto file to define the service

- touch time.proto

## Step 2:
Define the service definition in the proto file as per gRPC standard

- vim time.proto
- service time

## Step 3:
Generate the grpc files using the following command

```
python -m grpc_tools.protoc --python_out=. --grpc_python_out=. -I=. time.proto
```

The above command will generate 2 files:
- time_pb2.py
- time_pb2_grpc.py

## Step 4:
Create a server to serve the service defined

- touch server.py
- implement the service
- listen the server on a specified port

## Step 5:
Create a client to request the server

- touch client.py
- implement the client interface
- request the service specified in the specification

## Step 6:
Run the server and client. Client will get serviced from the server