# OSI_Model



Table of contents:


- [What is the OSI model?](#what-is-the-osi-model)
- [OSI model layers](#osi-model-layers)
   - [Layer-7 the application layer](#layer-7-the-application-layer)
   - [Layer-6 the presentation layer](#layer-6-the-presentation-layer)
   - [Layer-5 the session layer](#layer-5-the-session-layer)
   - [Layer-4 the transport layer](#layer-4-the-transport-layer)    
   - [Layer-3 the network layer](#layer-3-the-network-layer)
   - [Layer-2 the data link layer](#layer-2-the-data-link-layer)
   - [Layer-1 the physical layer](#layer-1-the-physical-layer)
  


## What is the OSI model?

**The Open Systems Interconnection (OSI) model** defines and used to understand
how to transferred from one computer to another in a computer network. In basic, 
two computer connected to each other with LAN cable and connectors with the help 
of Network Interface Cards(NICs).


## OSI model layers


7 layered OSI Model introducted by Interntional Organsation for Standardization 
is 1984.
Containing - Application layer, Presentation layer, Session layer, Transport layer,
             Network layer, Datalink layer, Physical layer.



#### Layer-7 the application layer

It is used by network application like Chrome, Firefox, Outlook etc.
Web browser is network application running in your PC. It does not 
reside in application layer. but it used application layer protocol 
HTTP and HTTPS - to do web suffering. there are dozen of application 
layer protocols that enables various function at this layer.
File tranfer, Web Suffer, Email with the helps of FTP protocol,
HTTP/HTTPS protocol, SMTP protocol respectively.




#### Layer-6 the presentation layer

It recieve data from application layer. this data is in form of characters and
numbers. it converts these character and number to machine understable binary 
format. This function of presentation layer is called translation. before 
transmitted the data , it reduces the number of bits that are used to represent 
the original data compression .the bit reducation is called data compression.
used to help data transmission can be done faster. Thus, data compession is very helpful in real time 
video and audio streaming.

To maintain the integrity of data, before transmission, data is encrypted. 
Encryption enchanes the security of the sensitive data. SSL protocol is 
used in presentation layer for encryption and decryption. 

So , it performs 3 basic function-
1. Transmission
2. Compression
3. Encryption/Decryption 

#### Layer-5 the session layer

It helps in setting up and managing connections enabling 
sending and recieving of data followed by termination of conection
and sessions. It has its own helper called APIs which allows application
on different computer to communicate with each other.

Just before a session or a connection is established  with a server. 
server performs a function called authentication. Authentication is the process 
of verify of computer address/ server. after authentiction the user, Authorizration
is the process used to determine is you have permission to access or not. session layer keeps 
a tracks of the file are recieved in the form of data packets. sessions layer keeps track everything of data packect.


#### Layer-4 the transport layer

It controls the reliablity of communication through segmentation, flows control
and error control. in segmentation, data recieved from sessions layer in dived into
 small data units called segments.
 each segment contains a source and destination port number and sequence number.
 port no. helps to direct smaller data used to correct application.
 Sequence no. helps to reassemble the segment in correct order to form correct message to reciever.
 protocols of transport layer are Transmission Control Protocol(TCP) and User Datagram Protocol(UDP).
 
 Transport Layer Provides two types of services -
 1. Connection - oriented Trabsmission
 2. Connetionless Transmission
 
 Connection-oriented transmission is done via TCP while Connectionless transmission is done via UDP.
 Transport layer passes data segments to the network layer.
 
 
 
#### Layer-3 the network layer

The network layer handles addressing and provides routing for messages or packets.
Since not all devices are directly connected to each other, some
packets may require multiple hops to get from source to destination.
Finding the way for packets in a large and variable network
is the job of the network layer. IP is a network layer protocol and IP address
is the IP address used to determine where packets should go. Addressing and routing of the
logical network occurs in the network layer. Layer 3 routers and switches
are devices that operate at the network layer.

#### Layer-2 the data link layer 

This layer communicates through blocks of data called frames. The data link
layer can perform error checking and information rate control. The data link
layer is for a wire with only two ends, a transmitter and a receiver. An 
exception is when the subclass is called the media access subclass is used.
This subclass is needed when frames conflict because multiple entities are 
trying to use the medium at the same time. This sublayer arbitrates collisions
to provide intact frames that the rest of the data link layer can use.
Bridges and switches manipulate data in the data link layer.

#### Layer-1 the physical layer

This layer includes the physical devices involved in data transmission, 
such as cables and switches. This is also the layer where data is 
converted to a bit stream, which is a sequence of 1s and 0s. The 
physical layer of both devices must also agree on the signal convention 
to be distinguishable. the numbers 1 and 0 on both devices devices.


