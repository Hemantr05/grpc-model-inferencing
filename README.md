# grpc-model-inferencing
Model inferencing using gRPC instead of the usual REST framework


## What is gRPC?
gRPC is a Remote Procedure Call (RPC) framework that runs on any device. gRPC is mainly developed and maintained by Google and it's widely used in the industry. It allows two machines to communicate, similar to HTTP, but with better syntax and performance. It's used to define microservices that may use different programming languages.

gRPC works by defining the fields of the messages the client and server will exchange and the signature of the function we will expose, with a special syntax in a .proto file, then gRPC generates both client and server code and you can call the function directly from the client.

gRPC services send and receive data as Protocol Buffer (Protobuf) messages, they can be better compressed than human-readable format (like JSON or XML), thus the better performance.

## Getting Started

Let's start by setting up a virtual environment in which we can build our project: <br>
```
$ python -m venv .venv
```

Then, let's install all the required packages,  <br>
```
$ pip install -r requirements.txt
```

## Run server

```
$ python src/client.py
```

Code from: https://blog.roboflow.com/deploy-machine-learning-models-pytorch-grpc-asyncio/
