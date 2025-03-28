# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.
## PROGRAM
CLIENT
```
import socket s=socket.socket() 
s.connect(('localhost',8000)) while True: 
    msg=input("Client > ")     s.send(msg.encode())     print("Server > ",s.recv(1024).decode())  
```
SERVER
```
import socket s=socket.socket() 
s.bind(('localhost',8000)) 
s.listen(5) c,addr=s.accept() while True: 
    ClientMessage=c.recv(1024).decode()     c.send(ClientMessage.encode()) 
```
## OUPUT
![Screenshot 2025-03-28 112223](https://github.com/user-attachments/assets/dffcec49-3d9b-4c3c-9754-94ecb4724fc6)

![Screenshot 2025-03-28 112233](https://github.com/user-attachments/assets/a4f41b2d-11e8-492b-98be-de1ab99e82b4)

## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
