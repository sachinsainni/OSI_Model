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
 - [References Section](#references)


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
             
![OSI model layer](https://user-images.githubusercontent.com/88798008/177087665-a8159a77-2294-45c5-b565-c38908c75f02.jpg)
<div align="center">
<p><strong>Figure:</strong> the OSI layers and their usage.</p>
</div>



#### Layer-7 the application layer

![application-layer](https://user-images.githubusercontent.com/88798008/177087948-9ac22f44-551a-4473-b194-eb69cc6d1e6c.svg)
<div align="center">
<p><strong>Figure:</strong> Application layer.</p>
</div>

It is used by network application like Chrome, Firefox, Outlook etc.
Web browser is network application running in your PC. It does not 
reside in application layer. but it used application layer protocol 
HTTP and HTTPS - to do web suffering. there are dozen of application 
layer protocols that enables various function at this layer.
File tranfer, Web Suffer, Email with the helps of FTP protocol,
HTTP/HTTPS protocol, SMTP protocol respectively.




#### Layer-6 the presentation layer

![6-presentation-layer](https://user-images.githubusercontent.com/88798008/177088028-81a0bca9-beef-4d4a-a0c8-e7118d44cb0b.svg)
<div align="center">
<p><strong>Figure:</strong> Presentation layer.</p>
</div>

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

![5-session-layer](https://user-images.githubusercontent.com/88798008/177088090-e220339d-ce95-4d34-82e9-ab26da4aca8e.svg)
<div align="center">
<p><strong>Figure:</strong> Session layer.</p>
</div>

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

![4-transport-layer](https://user-images.githubusercontent.com/88798008/177088181-871e8ed8-2e9e-434e-a420-913a9b850fc5.svg)
<div align="center">
<p><strong>Figure:</strong> Transport layer.</p>
</div>


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

![3-network-layer](https://user-images.githubusercontent.com/88798008/177088230-4ff42551-6a48-46d3-975b-43acbfc2647e.svg)
<div align="center">
<p><strong>Figure:</strong> Network layer.</p>
</div>

The network layer handles addressing and provides routing for messages or packets.
Since not all devices are directly connected to each other, some
packets may require multiple hops to get from source to destination.
Finding the way for packets in a large and variable network
is the job of the network layer. IP is a network layer protocol and IP address
is the IP address used to determine where packets should go. Addressing and routing of the
logical network occurs in the network layer. Layer 3 routers and switches
are devices that operate at the network layer.

#### Layer-2 the data link layer 

![2-data-link-layer](https://user-images.githubusercontent.com/88798008/177088384-e6b9b8ca-f2bf-4cc6-a419-341915c281fe.svg)
<div align="center">
<p><strong>Figure:</strong> Data link layer.</p>
</div>

This layer communicates through blocks of data called frames. The data link
layer can perform error checking and information rate control. The data link
layer is for a wire with only two ends, a transmitter and a receiver. An 
exception is when the subclass is called the media access subclass is used.
This subclass is needed when frames conflict because multiple entities are 
trying to use the medium at the same time. This sublayer arbitrates collisions
to provide intact frames that the rest of the data link layer can use.
Bridges and switches manipulate data in the data link layer.

#### Layer-1 the physical layer

![1-physical-layer](https://user-images.githubusercontent.com/88798008/177088492-11bae9ba-57da-4964-b425-7637793d37df.svg)
<div align="center">
<p><strong>Figure:</strong> Physical Layer.</p>
</div>

This layer includes the physical devices involved in data transmission, 
such as cables and switches. This is also the layer where data is 
converted to a bit stream, which is a sequence of 1s and 0s. The 
physical layer of both devices must also agree on the signal convention 
to be distinguishable. the numbers 1 and 0 on both devices devices.




## References

- [What is the OSI model?](https://www.cloudflare.com/learning/ddos/glossary/open-systems-interconnection-model-osi/)
- [OSI Model – Cheatsheet](https://www.routeralley.com/guides/osi.pdf)
- [OSI Model Explained](https://www.youtube.com/watch?v=vv4y_uOneC0&t=552s)
