# Experiment 6 - Echo client/server (Iterative)

## Description

An iterative server handles both the connection request and the transaction involved in the call itself.The server maintains one thread and responds with it. Multiple requests are queued for response, and dealt with in a FIFO manner.Iterative servers are fairly simple and are suitable for transactions that do not last long.

## Working

1. Client sends string size to server
2. Client sends string to server
3. Server sends string back to client

## Commands used for Execution

**server side**

gcc echo_server.c -o server
./server

**client side**

gcc echo_client.c -o client
./client

## Output

![3 diffrent inputs for the echo server-client](Echo server-client.png)

