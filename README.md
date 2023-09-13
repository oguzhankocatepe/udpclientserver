# udpclientserver
UDP Server-Client implementation in C++
Theory: In UDP, the client does not form a connection with the server like in TCP and instead sends a datagram. Similarly, the server need not accept a connection and just waits for datagrams to arrive. Datagrams upon arrival contain the address of the sender which the server uses to send data to the correct client. 
The entire process can be broken down into the following steps : 

UDP Server :  

Create a UDP socket.
Bind the socket to the server address.
Wait until the datagram packet arrives from the client.
Process the datagram packet and send a reply to the client.
Go back to Step 3.
UDP Client :  

Create a UDP socket.
Send a message to the server.
Wait until a response from the server is received.
Process the reply and go back to step 2, if necessary.
Close socket descriptor and exit.
