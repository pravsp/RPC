# Simple rpyc Example

## Step 1:
Create a server to serve the service defined

- touch server.py
- implement the service
- prefix the rpc call with export_
- listen the server on a specified port
- start the server with rpyc.ThreadedServer

## Step 2:
Create a client to request the server

- touch client.py
- implement the client interface
- request the service exported in the server
- connect to the server with rpyc.connect()

## Step 3:
Run the server and client. Client will get serviced from the server