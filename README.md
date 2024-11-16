# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# NAME: HARSSHITHA LAKSHMANAN
# REGNO: 212223230075
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
CLIENT:
```
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
    msg=input("Client> ")
    s.send(msg.encode())
    print("Server> ",s.recv(1024).decode())
```

SERVER:
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
## OUTPUT
## SERVER:

![WhatsApp Image 2024-09-19 at 10 37 03_11c5e715](https://github.com/user-attachments/assets/2297f137-0e1e-4049-b1e5-728e3d3f9dd8)


## CLIENT:

![WhatsApp Image 2024-09-19 at 10 36 52_82c1c401](https://github.com/user-attachments/assets/690762bf-cecb-4006-9591-3b5561181aeb)
## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
