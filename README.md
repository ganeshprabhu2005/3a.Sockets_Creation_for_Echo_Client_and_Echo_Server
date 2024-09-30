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
NAME:GANESH PRABHU J
REG NO:212223220023

## PROGRAM
```
import socket
s=socket.socket()
s.bind(('localhost',8000))
s.listen(5)
c,addr=s.accept()
while True:
 ClientMessage=c.recv(1024).decode()
 c.send(ClientMessage.encode())
```
```
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
 msg=input("Client > ")
 s.send(msg.encode())
 print("Server > ",s.recv(1024).decode())
```
## OUPUT
![370122370-cd6def60-bb5f-4802-8d78-adfc6611c0c9](https://github.com/user-attachments/assets/994bae57-793d-4b98-96e5-08ed60e4aede)


![370122422-dda8797d-0e52-4438-9ea0-94c5a6d6a2d3](https://github.com/user-attachments/assets/0320e85d-7aeb-4fdb-a821-69b60616490f)



## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
