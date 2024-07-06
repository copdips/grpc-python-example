# gRPC with Python Example

Doc from : <https://medium.com/@coderviewer/simple-usage-of-grpc-with-python-f714d9f69daa>

This repository contains a simple example of using gRPC (gRPC Remote Procedure Calls) with Python. The example demonstrates a basic client-server application where the server adds two numbers.

![Alt Text](logic.png)

## Getting Started

Follow the steps below to run the example on your local machine.

### Prerequisites

- Python (version 3.8 or higher)
- [grpcio](https://grpc.io/docs/quickstart/python/) and [grpcio-tools](https://grpc.io/docs/quickstart/python/#generate-code) installed

### Installing Dependencies

```bash
pip install grpcio grpcio-tools
```

### Generating gRPC files

```bash
python -m grpc_tools.protoc -I. --python_out=. --grpc_python_out=. calculator.proto
```

### Running the Server

```bash
python server.py
```

### Running the Client

```bash
python client.py
```
