# Experiment 5 - Implementation of concurrent chat server that allows current logged in users to communicate one with other

## Steps

  #Server
  
  Include appropriate header files.
1.Create a TCP Socket.
2.Fill in the socket address structure (with server information)
3.Bind the address and port using bind()system call.
4.Server executes listen()system call to indicate its willingness to receive connections.
5.Accept  the  next  completed  connection  from  the  client  process  by  using  an accept()system call.
6.Receive a message from the Client using recv()system call. 
7.Send the reply of the message madeby the client using send() system call

  #Client
  
  Create a TCP Socket.
1.Fill in the socket address structure (with server information)
2.Establish connection to the Server using connect()system call.
3.Send a chat message to the Server using send()system call.
4.Receive the reply message made to the server using recv() system call. 
5.Write the result thus obtained on the standard output.


## Commands used for Execution

**server side**

gcc server.c -o server  

./server 

**client side**

gcc client.c -o client  

./client 

## Output

![3 diffrent inputs for the chat box](https://github.com/Ayushkumar036/Network-Programming-and-Security-Lab/blob/main/Experiment%205-Part%20A/exp5.png?raw=true)



