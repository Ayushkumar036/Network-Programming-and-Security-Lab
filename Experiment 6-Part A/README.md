# Experiment 6 - Echo client/server (TCP/UDP)


## TCP ITERATIVE

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

![3 diffrent inputs for the echo server-client(TCP Iterative)](https://github.com/Ayushkumar036/Network-Programming-and-Security-Lab/blob/main/Experiment%206-Part%20A/Echo%20server-client.png?raw=true)


## TCP CONCURRENT

## Description

A concurrent server handles multiple clients at the same time. The simplest technique for a concurrent server is to call the fork function, creating one child process for each client. An alternative technique is to use threads instead (i.e., light-weight processes). 

## Working

When a connection is established, accept returns, the server calls fork, and the child process services the client (on the connected socket connfd). The parent process waits for another connection (on the listening socket listenfd. The parent closes the connected socket since the child handles the new client.

## Commands used for Execution

**server side**

gcc echo_server_concurrent.c -o server  

./server

**client side**

gcc echo_client_concurrent.c -o client  

./client 127.0.0.1

## Output

![3 diffrent inputs for the echo server-client(TCP Concurrent)](https://github.com/Ayushkumar036/Network-Programming-and-Security-Lab/blob/main/Experiment%206-Part%20A/TCP%20CONCURRENT.png?raw=true)

## UDP ITERATIVE

## Description

In UDP, the client does not form a connection with the server like in TCP and instead just sends a datagram. Similarly, the server need not accept a connection and just waits for datagrams to arrive. Datagrams upon arrival contain the address of sender which the server uses to send data to the correct client.

## Working


    1.Create UDP socket. 
    2.Bind the socket to server address.
    3.Wait until datagram packet arrives from client.
    4.Process the datagram packet and send a reply to client.
    5.Go back to Step 3.


## Commands used for Execution

**server side**

gcc echo_server_udp.c -o server  

./server 8000

**client side**

gcc echo_client_udp.c -o client  

./client localhost 8000

## Output

![3 diffrent inputs for the echo server-client(UDP Iteartive)](https://github.com/Ayushkumar036/Network-Programming-and-Security-Lab/blob/main/Experiment%206-Part%20A/UDP%20ITERATIVE.png?raw=true)



