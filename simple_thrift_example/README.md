# Simple thrift Example

## Pre-Requisite
- thrift binary to be available (install using ```brew install thrift``` in case of mac-os)
- install the requirements.txt file containing python dependancies

## Step 1:
Create a thrift file to define the service

- touch time_service.thrift

## Step 2:
Define the service definition in the thrift file as per thrift IDL standard

- vim time_service.thrift
- service TimeService

## Step 3:
Generate the thrift files using the following command

```
thrift -r --gen py time_service.thrift
```

The above command will generate gen-py folder containing the thrift auto generated code.

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

# Simple thriftpy approach

An alternate approach for thrift client is to use thriftpy pakcakge.

- Create the simple server endpoint as defined in thriftpy_approach/server.py
- Create simple client endpoint as defined in thriftpy_approach/client.py
- run the server and client to request service from server